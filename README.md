# ZzFX - Zuper Zmall Zound Zynth

# [ZzFX Sound Designer](https://zzfx.3d2k.com)
# [ZzFX Sound Board Demo](https://codepen.io/KilledByAPixel/full/BaowKzv)

### ZzFX is a JavaScript sound effect engine and creation tool supported by most modern broswers.

- Sound effects can be generated or manually created using the web based sound effect creation tool.

- Just include ZzFX.min.js to load ZzFX, it does not need to be initialized.

- Or you can use ZzFX.micro.js a tiny (<1k) version that has only the ability to play sounds.

To play a sound in code, just call a simple function! Here are some examples...

```
zzfx(...[,,537,.02,.02,.22,1,1.59,-6.98,4.97]); // Heart
zzfx(...[,,925,.04,.3,.6,1,.3,,6.27,-184,.09,.17]); // Game Over
zzfx(...[,,539,,.04,.29,1,1.92,,,567,.02,.02,,,,.04]); // Twinkle
zzfx(...[,0,1600,.13,.52,.61,1,1.1,,,,,,.1,,.14]); // Phone Ring
zzfx(...[,,709,,,.07,,,,3.7,,,,3.6,,,.11]); // Echo Click
zzfx(...[1.5,.8,270,,.1,,1,1.5,,,,,,,,.1,.01]); // Piano
zzfx(...[,,129,.01,,.15,,,,,,,,5]); // Drum
```

### Here's the code for the ZzFXmicro, this all you need to play ZzFX sounds!

```
zzfxV=.3 // volume
zzfx=    // play sound
(H=1,I=.05,g=220,J=0,K=0,L=.1,l=0,M=1,q=0,N=0,O=0,P=0,Q=0,v=0,w=0,R=0,S=0,r=1,T=0,d=2*Math.PI,b=44100,t=m=>2*m*Math.random()-m,x=m=>0<m?1:-1,U=q*=500*d/b**2,V=x(w)*d/4,y=g*=(1+t(I))*d/b,f=99+J*b|0,n=T*b|0,z=K*b|0,A=L*b|0,e=S*b|0,W=500*N*d/b**3,X=w*d/b,B=O*d/b,Y=P*b,C=Q*b,h=f+n+z+A+e,p=[],D=0,E=0,c=0,k=1,F=0,G=0,a=0,Z,u=zzfxX.createBufferSource())=>{for(;c<h;p[c++]=a)++G>100*R&&(G=0,a=D*g*Math.sin(E*X-V),a=l?1<l?2<l?3<l?Math.sin((a%d)**3):Math.max(Math.min(Math.tan(a),1),-1):1-(2*a/d%2+2)%2:1-4*Math.abs(Math.round(a/d)-a/d):Math.sin(a),a=x(a)*Math.abs(a)**M,a*=H*zzfxV*(c<f?c/f:c<f+n?1-(c-f)/n*(1-r):c<f+n+z?r:c<h-e?(h-c-e)/A*r:0),a=e?a/2+(e>c?0:(c<h-e?1:(c-h)/e)*p[c-e]/2):a),D+=1+t(v),E+=1+t(v),g+=q+=W,k&&++k>Y&&(g+=B,y+=B,k=0),C&&++F>C&&(g=y,q=U,F=1,k=k||1);buffer=zzfxX.createBuffer(1,p.length,b);buffer.getChannelData(0).set(p);u.buffer=buffer;u.connect(zzfxX.destination);u.start()};zzfxX=new AudioContext
```

![ZzFX Image](/screenshot.jpg)

## ZzFX Features

- Tiny synth engine with 17 controllable parameters.
- Play sounds via code, no need for sound asset files!
- Compatible with nearly all web browsers.
- Small code footprint, the micro version is under 1 kilobyte.
- Can produce a massive variety of sound effect types.
- Sounds can be played with a short call. zzfx(...[,,,,.1,,,,9])
- Use ZZFX.GetNote to get frequencies on a standard diatonic scale.
- Supports saving sounds as wav files for offline playback.
- Both ZzFX and ZzFXMicro run in strict mode.
- No additional libraries or dependencies are required.
- Open source with MIT license, you can use this for anything!

## ZzFX UI Features

- Generates random sounds from presets.
- Sound list is saved automatically.
- Each parameter can be modified with constraints.
- Lock and mutate buttons for each parameter.
- Sound name can be changed for easier workflow.
- Shortens code for zzfx sound calls.
- Displays image of sound wave when played.
- Sounds can be download as a wave file.
- Sounds can be marked as favorites to prevent removal.
- Sounds can be loaded by pasting zzfx code for easy sharing.
- List of sounds can be exported and imported.
- Supports drag-and-drop of exported files into sound list.

## Games Using ZzFX

- [Bogus Roads](https://www.newgrounds.com/portal/view/747570)
- [The Wandering Wraith](https://js13kgames.com/entries/the-wandering-wraith)
- [Bounce Back](https://js13kgames.com/entries/bounce-back)
- [Egg Time Rewind](https://killedbyapixel.itch.io/egg-time)
- [Hue Jumper](https://killedbyapixel.itch.io/hue-jumper)
- [Bubba's Back Room](https://js13kgames.com/entries/bubbas-back-room)
- [Backstabber Hero](https://js13kgames.com/entries/backstabber-hero)
- [Spendotron: 2019](https://killedbyapixel.itch.io/currency-wars)
- [Dioretsa](https://js13kgames.com/entries/20461-dioretsa)
- [Back 2 Back](https://js13kgames.com/entries/back-2-back)
- [Quick Wins](https://js13kgames.com/entries/quick-wins)
- [Back Relax](http://js13kgames.com/entries/back-relax)
- [Back To The Island](https://js13kgames.com/entries/back-to-the-island)
- [Backspace It](http://js13kgames.com/entries/backspace-it)
- [Back To The Stars](https://js13kgames.com/entries/back-to-the-stars)
- [Can't Get Back](https://js13kgames.com/entries/cant-get-back)
- [Letchworth Village](https://js13kgames.com/entries/letchworth-village)
- [Noegnud](https://js13kgames.com/entries/noegnud)
- [Sausage Redemption](https://gogoprog.itch.io/sausage-redemption)
- [Marshmallow Sky](https://github.com/baturinsky/marshmallow-sky) 

## [ZzFX Community Soundboard](https://codepen.io/KilledByAPixel/full/dyYVwGP)

- Just for fun I created a soundboard where everyone can have one sound.
- Send me a zzfx code and emoji to get your sound added!

![ZzFX Image](/favicon.png) 
