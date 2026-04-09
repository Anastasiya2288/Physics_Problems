# 9. Damped Oscillator

## 📘 Key Definitions and Formulas

### 1. Differential Equation

$$m\frac{d^2x}{dt^2}+b\frac{dx}{dt}+kx=0$$

---

### 2. Standard Form

Divide by $m$:

$$\frac{d^2x}{dt^2}+\frac{b}{m}\frac{dx}{dt}+\frac{k}{m}x=0$$

Define:

- Natural frequency: $$\omega_0=\sqrt{\frac{k}{m}}$$
- Damping coefficient: $$\gamma=\frac{b}{2m}$$

---

### 3. Characteristic Equation

$$r^2+2\gamma r+\omega_0^2=0$$

---

## 🧠 1. General Solution

### 🔹 Underdamped $$\gamma<\omega_0$$

$$x(t)=A e^{-\gamma t}\cos(\omega_d t+\phi)$$

where:

$$\omega_d=\sqrt{\omega_0^2-\gamma^2}$$

---

### 🔹 Critically Damped $$\gamma=\omega_0$$

$$x(t)=(A+Bt)e^{-\gamma t}$$

---

### 🔹 Overdamped $$\gamma>\omega_0$$

$$x(t)=A e^{r_1 t}+B e^{r_2 t}$$

where:

$$r_{1,2}=-\gamma\pm\sqrt{\gamma^2-\omega_0^2}$$

---

## 🧠 2. Classification

- Underdamped → oscillations with decay  
- Critically damped → fastest return without oscillation  
- Overdamped → slow return, no oscillation  

---

## 🧮 3. Numerical Solution $$RK4$$

We convert to system:

$$\frac{dx}{dt}=v$$  
$$\frac{dv}{dt}=-\frac{b}{m}v-\frac{k}{m}x$$

---

## 💻 4–6. Interactive HTML (RK4 + Slider + Graphs)

```html
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Damped Oscillator</title>
<style>
body { font-family: Arial; text-align: center; }
canvas { border:1px solid black; margin:10px; }
</style>
</head>
<body>

<h2>Damped Oscillator Simulation</h2>

<label>Damping b: </label>
<input type="range" min="0" max="20" step="0.1" value="2" id="slider">
<span id="bVal">2</span>

<br><br>

<canvas id="xt" width="400" height="200"></canvas>
<canvas id="phase" width="400" height="200"></canvas>

<script>
const m=1;
const k=10;

function rk4(x,v,dt,b){
    function ax(x,v){ return v; }
    function av(x,v){ return -(b/m)*v-(k/m)*x; }

    let k1x=dt*ax(x,v);
    let k1v=dt*av(x,v);

    let k2x=dt*ax(x+k1x/2,v+k1v/2);
    let k2v=dt*av(x+k1x/2,v+k1v/2);

    let k3x=dt*ax(x+k2x/2,v+k2v/2);
    let k3v=dt*av(x+k2x/2,v+k2v/2);

    let k4x=dt*ax(x+k3x,v+k3v);
    let k4v=dt*av(x+k3x,v+k3v);

    x += (k1x+2*k2x+2*k3x+k4x)/6;
    v += (k1v+2*k2v+2*k3v+k4v)/6;

    return [x,v];
}

function simulate(b){
    let x=1, v=0;
    let dt=0.02;
    let data=[];
    for(let t=0;t<20;t+=dt){
        data.push([t,x,v]);
        [x,v]=rk4(x,v,dt,b);
    }
    return data;
}

function draw(){
    let b=parseFloat(slider.value);
    document.getElementById("bVal").innerText=b;

    let data=simulate(b);

    let ctx1=xt.getContext("2d");
    ctx1.clearRect(0,0,400,200);

    ctx1.beginPath();
    data.forEach((p,i)=>{
        let x=i;
        let y=100-p[1]*80;
        if(i===0) ctx1.moveTo(x,y);
        else ctx1.lineTo(x,y);
    });
    ctx1.stroke();

    let ctx2=phase.getContext("2d");
    ctx2.clearRect(0,0,400,200);

    ctx2.beginPath();
    data.forEach((p,i)=>{
        let x=200+p[1]*80;
        let y=100-p[2]*40;
        if(i===0) ctx2.moveTo(x,y);
        else ctx2.lineTo(x,y);
    });
    ctx2.stroke();
}

slider.oninput=draw;
draw();
</script>

</body>
</html>
```

---

## 🎯 Final Insight

✔️ Small $b$ → oscillations (underdamped)  
✔️ Medium $b$ → fastest stabilization (critical)  
✔️ Large $b$ → slow return (overdamped)  

✔️ Phase portrait clearly shows:
- spirals → underdamped  
- straight decay → overdamped  
- boundary case → critical  

✔️ RK4 provides accurate numerical simulation of the system dynamics.