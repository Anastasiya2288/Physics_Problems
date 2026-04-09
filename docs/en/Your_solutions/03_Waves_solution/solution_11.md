# 11. Animation: Two-Slit Interference

## 📘 Key Definitions and Formulas

### 1. Wave from Each Slit

$$u_1=\frac{A}{|\vec{r}-\vec{r_1}|}\sin(k|\vec{r}-\vec{r_1}|-\omega t)$$  
$$u_2=\frac{A}{|\vec{r}-\vec{r_2}|}\sin(k|\vec{r}-\vec{r_2}|-\omega t)$$

---

### 2. Superposition Principle

$$u_{total}=u_1+u_2$$

---

### 3. Distance Formula

$$|\vec{r}-\vec{r_i}|=\sqrt{(x-x_i)^2+(y-y_i)^2}$$

---

### 4. Wave Parameters

$$k=\frac{2\pi}{\lambda}$$  
$$\omega=2\pi f$$

---

### 5. Interference Condition

- Constructive: path difference $=n\lambda$  
- Destructive: path difference $=\frac{(2n+1)\lambda}{2}$  

---

## 🧠 Step-by-Step Idea

1. Two fixed sources $\vec{r_1},\vec{r_2}$  
2. Distance between them: $d$ (controlled by slider)  
3. For each pixel:
   - compute distances $r_1,r_2$
   - compute waves
   - sum them  
4. Animate time evolution  
5. Visualize intensity  

---

## 💻 Interactive HTML Animation

```html
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Two-Slit Interference</title>
<style>
body { text-align:center; font-family:Arial; }
canvas { border:1px solid black; }
</style>
</head>
<body>

<h2>Two-Slit Interference</h2>

<label>Slit distance d:</label>
<input type="range" min="20" max="200" value="80" id="dSlider">
<span id="dVal">80</span>

<br>

<label>Wavelength λ:</label>
<input type="range" min="10" max="100" value="40" id="lambdaSlider">
<span id="lambdaVal">40</span>

<br><br>

<canvas id="canvas" width="500" height="500"></canvas>

<script>
const canvas = document.getElementById("canvas");
const ctx = canvas.getContext("2d");

let t = 0;
const A = 1;
const omega = 0.15;

function draw(){

    let d = parseFloat(dSlider.value);
    let lambda = parseFloat(lambdaSlider.value);

    document.getElementById("dVal").innerText = d;
    document.getElementById("lambdaVal").innerText = lambda;

    let k = 2*Math.PI / lambda;

    let r1 = { x: 250, y: 250 - d/2 };
    let r2 = { x: 250, y: 250 + d/2 };

    let img = ctx.createImageData(canvas.width, canvas.height);

    for(let x=0;x<canvas.width;x+=2){
        for(let y=0;y<canvas.height;y+=2){

            let dx1 = x - r1.x;
            let dy1 = y - r1.y;
            let dist1 = Math.sqrt(dx1*dx1 + dy1*dy1) + 0.0001;

            let dx2 = x - r2.x;
            let dy2 = y - r2.y;
            let dist2 = Math.sqrt(dx2*dx2 + dy2*dy2) + 0.0001;

            let u1 = (A / dist1) * Math.sin(k*dist1 - omega*t);
            let u2 = (A / dist2) * Math.sin(k*dist2 - omega*t);

            let u = u1 + u2;

            let color = Math.floor(128 + 127*u);

            let index = (y*canvas.width + x)*4;
            img.data[index] = color;
            img.data[index+1] = color;
            img.data[index+2] = 255 - color;
            img.data[index+3] = 255;
        }
    }

    ctx.putImageData(img,0,0);

    // draw slit points
    ctx.fillStyle = "red";
    ctx.beginPath();
    ctx.arc(r1.x, r1.y, 4, 0, 2*Math.PI);
    ctx.fill();

    ctx.beginPath();
    ctx.arc(r2.x, r2.y, 4, 0, 2*Math.PI);
    ctx.fill();

    t += 1;
    requestAnimationFrame(draw);
}

draw();
</script>

</body>
</html>
```

---

## 🎯 Final Insight

✔️ Changing $d$:
- Larger $d$ → more closely spaced fringes  

✔️ Changing $\lambda$:
- Larger $\lambda$ → wider fringes  

✔️ Bright regions → constructive interference  
✔️ Dark regions → destructive interference  

✔️ This simulation reproduces **Young’s double-slit experiment in real time**