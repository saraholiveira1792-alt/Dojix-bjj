# Dojix-bjj
DOJIX BJJ — Jogo 3D de Jiu-Jitsu Brasileiro`
show('ESCAPE EXECUTADO!');
 save();
}

function save(){
 localStorage.setItem('dojixXP',xp);
 updateHUD();
}

// Controlos tácteis
const joyArea=document.getElementById('joy');
const knob=document.getElementById('knob');

joyArea.addEventListener('pointerdown',e=>{
 joyArea.setPointerCapture(e.pointerId);
 moveJoy(e);
});

joyArea.addEventListener('pointermove',e=>{
 if(e.buttons)moveJoy(e);
});

function moveJoy(e){
 let r=joyArea.getBoundingClientRect();
 let x=(e.clientX-r.left-r.width/2)/43;
 let y=(e.clientY-r.top-r.height/2)/43;

 let d=Math.hypot(x,y);
 if(d>1){x/=d;y/=d;}

 joy={x,y};
 knob.style.left=(33+x*30)+'px';
 knob.style.top=(33+y*30)+'px';
}

function resetJoy(){
 joy={x:0,y:0};
 knob.style.left='33px';
 knob.style.top='33px';
}

joyArea.addEventListener('pointerup',resetJoy);
joyArea.addEventListener('pointercancel',resetJoy);

document.getElementById('attack').addEventListener('pointerdown',technique);
document.getElementById('takedown').addEventListener('pointerdown',takedown);
document.getElementById('escape').addEventListener('pointerdown',escape);

let db=document.getElementById('defend');

db.addEventListener('pointerdown',()=>{
 defending=true;
 show('DEFESA ATIVA');
});

db.addEventListener('pointerup',()=>defending=false);
db.addEventListener('pointercancel',()=>defending=false);
db.addEventListener('pointerleave',()=>defending=false);

// Jogo
function animate(){
 requestAnimationFrame(animate);

 let dt=Math.min(clock.getDelta(),.05);
 let t=clock.elapsedTime;

 if(active){

  // Movimento do atleta
  player.root.position.x+=joy.x*3*dt;
  player.root.position.z+=joy.y*3*dt;

  player.root.position.x=THREE.MathUtils.clamp(
   player.root.position.x,-4.5,4.5);

  player.root.position.z=THREE.MathUtils.clamp(
   player.root.position.z,-4.5,4.5);

  let moving=Math.abs(joy.x)+Math.abs(joy.y)>.1;

  player.arms.forEach((a,i)=>{
   a.rotation.x=moving?Math.sin(t*8+i)*.3:0;
  });

  // Inteligência artificial
  if(mode==='combate'){
   let dx=player.root.position.x-enemy.root.position.x;
   let dz=player.root.position.z-enemy.root.position.z;
   let d=Math.hypot(dx,dz);

   if(d>1.4){
    enemy.root.position.x+=dx/d*dt*1.1;
    enemy.root.position.z+=dz/d*dt*1.1;
   }

   aiCooldown-=dt;

   if(d<1.6 && aiCooldown<=0){
    aiCooldown=3;

    if(defending){
     show('BOA DEFESA!');
     xp+=5;
    }else{
     energy=Math.max(0,energy-10);
     show('O ADVERSÁRIO ATACOU!');
    }
    updateHUD();
   }

   if(energy<=0){
    active=false;
    show('COMBATE TERMINADO!');
   }
  }

  // Orientação dos lutadores
  let dx=enemy.root.position.x-player.root.position.x;
  let dz=enemy.root.position.z-player.root.position.z;

  player.root.rotation.y=Math.atan2(dx,dz);
  enemy.root.rotation.y=Math.atan2(-dx,-dz);

  // Câmara
  camera.position.x=player.root.position.x*.3;
  camera.lookAt(0,0,0);
 }

 if(msgTime>0){
  msgTime-=dt;
  if(msgTime<=0)
   document.getElementById('message').innerText='';
 }

 renderer.render(scene,camera);
}

init();
</script>
</body>
</html>
```


Depois vamos ativar o *GitHub Pages* para teres o teu próprio link do DOJIX BJJ! 🥋
