# <p align="center">FAST.COM prank script</p>

<p align="center">The simle JS script for pranking fast.com</p>

<div align="center">
  
  ![Screencastfrom21-04-24160404-ezgif com-video-to-gif-converter](https://github.com/musobekmadrimov/fast.com-prank-hack-function-/assets/66286036/36ddd21e-3c10-409e-bb3f-dabfcd030828)
  
</div>




All you need to do is just copy the code below and paste to Chrome console, opened in fast.com website.

```javascript
function hack(){
    let showMore = document.getElementById("show-more-details-link");
    let footerContainer = document.querySelector(".footer-container");
    let speedUnits = document.getElementById("speed-units");
    let firstSpeed = 3;
    let speedValue = document.getElementById("speed-value");
    let count = setInterval(() => {
        firstSpeed += Math.floor(Math.random() * 50);
        showMore.style.display = "none";
        footerContainer.style.display = "none";
      speedValue.style.color = "#d2d2d2";
        speedUnits.style.color = "#d2d2d2";
            speedValue.innerText = firstSpeed;
        if (firstSpeed >= 1000) {
            speedValue.innerText = (firstSpeed / 1000).toFixed(1);
            speedUnits.innerText = "Gbps";
            if (firstSpeed >= 1284) {
                speedValue.style.color = "#000";
                speedUnits.style.color = "#000";
                showMore.style.display = "block";
                footerContainer.style.display = "block";
                clearInterval(count);
            }
        } else {
            speedUnits.innerText = "Mbps";
        } 
          }, 100)
    
}

document.addEventListener("click", () => {
    hack();
})
```
That is it! Just click everywhere(_exept refresh button_) in the screen and enjoy! Try not to laugh at your friends' reaction! 😁

**Note:** _If browser console does not allow paste code write `allow paste` and it will allow. Happy pranking!_ 😉
