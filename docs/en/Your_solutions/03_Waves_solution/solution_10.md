# 10. Animation: Wave Sources

## 📘 Key Definitions and Formulas

### 1. Wave from a Point Source

$$u(\vec{r},t)=\frac{A}{|\vec{r}-\vec{r_0}|^\alpha}\sin(k|\vec{r}-\vec{r_0}|-\omega t)$$

Where:
- $A$ — amplitude  
- $\vec{r}$ — observation point  
- $\vec{r_0}$ — source position  
- $\alpha$ — attenuation factor  
- $k=\frac{2\pi}{\lambda}$ — wave number  
- $\omega=2\pi f$ — angular frequency  

---

### 2. Distance Between Points

$$|\vec{r}-\vec{r_0}|=\sqrt{(x-x_0)^2+(y-y_0)^2}$$

---

### 3. Superposition Principle

Total wave is the sum of all sources:

$$u_{total}=\sum_i u_i$$

---

## 🧠 Step-by-Step Idea

1. User clicks → adds a source $\vec{r_0}$  
2. For each pixel → compute distance to all sources  
3. Compute wave contribution  
4. Sum all contributions  
5. Animate in time  

---

## 💻 Interactive HTML Animation

```html
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Wave Sources</title>
<style>
body { text-align:center; font-family:Arial; }
canvas { border:1px solid black; }
</style>
</head>
<body>

<h2>Wave Superposition</h2>

<label>Alpha $$\alpha$$:</label>
<input type="range" min="0" max="2" step="0.1" value="1" id="alphaSlider">
<span id="alphaVal">1</span>

<br><br>
<canvas id="canvas" width="500" height="500"></canvas>

<script>
const canvas = document.getElementById("canvas");
const ctx = canvas.getContext("2d");

let sources = [];
let t = 0;

const A = 1;
const k = 0.1;
const omega = 0.1;

canvas.onclick = function(e){
    const rect = canvas.getBoundingClientRect();
    sources.push({
        x: e.clientX - rect.left,
        y: e.clientY - rect.top
    });
};

function draw(){
    let alpha = parseFloat(alphaSlider.value);
    document.getElementById("alphaVal").innerText = alpha;

    let img = ctx.createImageData(canvas.width, canvas.height);

    for(let x=0;x<canvas.width;x+=2){
        for(let y=0;y<canvas.height;y+=2){

            let u = 0;

            for(let s of sources){
                let dx = x - s.x;
                let dy = y - s.y;
                let r = Math.sqrt(dx*dx + dy*dy) + 0.0001;

                u += (A / Math.pow(r, alpha)) * Math.sin(k*r - omega*t);
            }

            let color = Math.floor(128 + 127*u);

            let index = (y*canvas.width + x)*4;
            img.data[index] = color;
            img.data[index+1] = color;
            img.data[index+2] = 255 - color;
            img.data[index+3] = 255;
        }
    }

    ctx.putImageData(img,0,0);

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

✔️ Each click creates a new wave source  
✔️ The animation shows **interference patterns**  
✔️ Changing $\alpha$ controls how fast waves decay:
- $\alpha=0$ → no decay  
- $\alpha=1$ → realistic spreading  
- $\alpha=2$ → strong attenuation  

✔️ The result demonstrates **real-time wave superposition and interference**