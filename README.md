<svg fill="none" viewBox="0 0 1200 750" width="1200" height="750" xmlns="http://www.w3.org/2000/svg">
	<foreignObject width="100%" height="100%">
		<div xmlns="http://www.w3.org/1999/xhtml">
			<style>
				@font-face {
                font-family: "Klingon pIqaD HaSta";
                src: url("https://assets.codepen.io/907471/Klingon-pIqaD-HaSta.ttf")
                    format("truetype");
                }

                #container {
                background: inherit;
                }

                body {
                background: black;
                height: 100vh;
                width: 100vw;
                color: #ea6161;
                overflow: hidden;
                }
			</style>

			<canvas id="container"></canvas>
		</div>
	</foreignObject>
</svg>
<script>
    const primaryColor = "#ea6161";
    const source = "";

    const getRndInteger = (min, max) =>
    Math.floor(Math.random() * (max - min + 1)) + min;
    let interval;

    const start = () => {
    const canvas = document.getElementById("container");
    const rect = canvas.parentElement.getBoundingClientRect();
    canvas.width = rect.width;
    canvas.height = rect.height;
    const ctx = canvas.getContext("2d");
    const size = 14;
    ctx.font = `${size}px "Klingon pIqaD HaSta"`;
    const columns = Math.round(canvas.width / size);
    const rows = Math.round(canvas.height / size);
    const columnCells = Array(columns)
        .fill(0)
        .map(() => getRndInteger(0, canvas.height));

    const render = () => {
        ctx.fillStyle = "rgba(0,0,0,.07)";
        ctx.fillRect(0, 0, canvas.width, canvas.height);
        ctx.fillStyle = primaryColor;
        columnCells.forEach((y, index) => {
        const text = source[getRndInteger(0, source.length + 2)] ?? "";
        const x = index * size;
        ctx.fillText(text, x, y);
        columnCells[index] =
            y > canvas.height + getRndInteger(0, 10000) ? 0 : y + size;
        });
    };

    interval = window.setInterval(render, 60);
    };

    (() => {
    start();

    window.addEventListener("resize", () => {
        clearInterval(interval);
        start();
    });
    })();

</script>
<h1 align="center">
    <img src="https://readme-typing-svg.herokuapp.com/?font=Righteous&size=35&center=true&vCenter=true&width=500&height=70&duration=4000&lines=Hi+There!+👋;+I'm+Viet+Anh!;" />
</h1>

# 🏄‍♂️ Viet Anh

**`Viet Anh (Developer)`**

## I'm an indie developer building my version of the digital world one step at a time. All coding projects are built from the ground up, from planning and designing all the way to solving real-life problems with code.

<img align="right" alt="Coding" width="400" src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExZjF6cDNzODI4bXlpZW14NHJoYXI1OHJrbjNqYmF0bmV6M3NmeTRjdyZlcD12MV9naWZzX3NlYXJjaCZjdD1n/RbDKaczqWovIugyJmW/giphy.gif">

- 🔭 I’m currently studying at **FPT Univesity**

- 🌱 I’m currently learning **Spring**

- 💬 Ask me about **Java , SQL**

### 🧰 Languages and Tools

<a href="https://azure.microsoft.com/en-in/" target="_blank" rel="noreferrer"> 
<img src="https://www.vectorlogo.zone/logos/microsoft_azure/microsoft_azure-icon.svg" alt="azure" width="40" height="40"/> </a> 
<a href="https://getbootstrap.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain-wordmark.svg" alt="bootstrap" width="40" height="40"/> </a> 
<a href="https://www.cprogramming.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/c/c-original.svg" alt="c" width="40" height="40"/> </a> 
<a href="https://www.w3schools.com/cpp/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/cplusplus/cplusplus-original.svg" alt="cplusplus" width="40" height="40"/> </a> 
<a href="https://www.w3schools.com/cs/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/csharp/csharp-original.svg" alt="csharp" width="40" height="40"/> </a> 
<a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> </a> 
<a href="https://dotnet.microsoft.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/dot-net/dot-net-original-wordmark.svg" alt="dotnet" width="40" height="40"/> </a> 
<a href="https://git-scm.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git" width="40" height="40"/> </a> <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a> <a href="https://www.java.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" alt="java" width="40" height="40"/> </a> 
<a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> </a> 
<a href="https://www.microsoft.com/en-us/sql-server" target="_blank" rel="noreferrer"> <img src="https://www.svgrepo.com/show/303229/microsoft-sql-server-logo.svg" alt="mssql" width="40" height="40"/> </a> 
<a href="https://postman.com" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/getpostman/getpostman-icon.svg" alt="postman" width="40" height="40"/> </a> 
<a href="https://spring.io/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/springio/springio-icon.svg" alt="spring" width="40" height="40"/> </a>
<br />

# 📊 GitHub Stats:
![](https://github-readme-stats.vercel.app/api?username=vietanh30021160&theme=dark&hide_border=false&include_all_commits=false&count_private=false)<br/>

<!-- Proudly created with GPRM ( https://gprm.itsvg.in ) -->