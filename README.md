<!DOCTYPE html><html lang="es"><head><meta charset="UTF-8"><meta name="viewport" content="width=device-width, initial-scale=1"><title>THE WIN - RIFA OFICIAL</title><style>body{margin:0;background:#000;color:#fff;font-family:system-ui}.wrap{max-width:480px;margin:auto;padding:12px}.card{border:1px solid #C5A028;border-radius:16px;background:#111;padding:16px;margin:12px 0}.bar{background:#222;height:28px;border-radius:20px;overflow:hidden;position:relative}.fill{height:100%;background:linear-gradient(90deg,#C5A028,#F9E27D);width:0%;transition:.8s}.barText{position:absolute;top:0;left:0;width:100%;height:100%;display:flex;align-items:center;justify-content:center;font-weight:900;font-size:13px;color:#fff}.grid{display:grid;grid-template-columns:repeat(8,1fr);gap:5px;max-height:340px;overflow-y:auto;background:#0a0a0a;padding:10px;border-radius:12px}.num{border:1px solid #C5A028;height:36px;display:flex;align-items:center;justify-content:center;font-size:10px;font-weight:800;background:#1a1a1a;border-radius:8px}.num.sel{background:#C5A028;color:#000}.num.vend{background:#3a0000;color:#666;text-decoration:line-through}.btn{width:100%;padding:16px;border:none;border-radius:14px;font-weight:900;background:linear-gradient(90deg,#C5A028,#F9E27D);color:#000;font-size:16px;cursor:pointer}input{width:93%;padding:12px;margin:6px 0;border-radius:10px;border:1px solid #333;background:#1a1a1a;color:#fff}.pagoBox{border:2px solid gold;background:#1a1a1a;border-radius:14px;padding:14px;margin:8px 0}#p2,#p3{display:none}</style></head><body><div class="wrap">

<div id="pantalla1">
<div style="text-align:center;padding:10px"><div style="width:80px;height:80px;margin:auto;border-radius:50%;background:linear-gradient(135deg,gold,#F9E27D);display:flex;align-items:center;justify-content:center;color:#000;font-weight:900">THE WIN</div><h1 style="margin:10px 0 0;color:gold">¡GRAN SORTEO!</h1><h2 style="margin:0">KEEWAY MINNIX 150</h2></div>

<div class="card" style="background:linear-gradient(135deg,#111,#1a1a1a);border-color:gold">
<h3 style="margin:0 0 10px;color:gold;text-align:center">🏆 PREMIOS</h3>
<p style="margin:6px 0">🏍️ 1er Premio: Moto Keeway Minnix 150 0km</p>
<p style="margin:6px 0">📱 2do Premio: iPhone 15</p>
<p style="margin:6px 0">⛑️ 3er Premio: Casco Certificado + Aceite</p>
<p style="margin:6px 0">🌐 Extra: 1 Año de Internet Gratis</p>
</div>

<div class="card">
<div style="display:flex;justify-content:space-between;margin-bottom:8px"><b>PROGRESO RIFA</b><b style="color:gold"><span id="vend1">0</span>/1000</b></div>
<div class="bar"><div class="fill" id="fill1"></div><div class="barText" id="porc1">0% VENDIDO</div></div>
<p style="text-align:center;font-size:12px;color:#aaa;margin:8px 0 0">¡Quedan pocos números!</p>
</div>

<div class="card" style="text-align:center">
<p style="margin:4px 0;font-size:14px">💲 VALOR POR NÚMERO</p><p style="margin:0;font-size:36px;font-weight:900;color:gold">$1,00</p><p style="margin:4px 0;font-size:12px;color:#aaa">Mínimo 5 números ($5)</p>
<hr style="border-color:#222;margin:12px 0">
<p style="margin:4px 0">📞 CONTACTO OFICIAL</p><p style="margin:0;font-size:20px;font-weight:900;color:#25D366">099 123 4567</p><p style="font-size:11px;color:#aaa">WhatsApp directo</p>
</div>

<button class="btn" onclick="irANumeros()" style="font-size:18px;padding:20px">🎟️ COMPRAR NÚMEROS →</button>
<p style="text-align:center;font-size:10px;color:#666">Sorteo por Lotería Nacional - 100% Legal</p>
</div>

<div id="p2">
<button onclick="irAPrincipal()" style="background:#222;color:#fff;border:1px solid #444;border-radius:8px;padding:8px 12px;margin-bottom:10px">← VOLVER</button>
<h3 style="text-align:center;color:gold;margin:0">ELIGE TUS NÚMEROS</h3>
<div class="card"><div style="display:flex;justify-content:space-between"><span>Vendidos: <b id="vend2">0</b>/1000</b></span><button onclick="autoSel()" style="background:#222;color:gold;border:1px solid gold;border-radius:6px;padding:4px 8px;font-size:10px">🎲 ALEATORIO 5</button></div><div class="grid" id="grid"></div><p style="text-align:center">Sel: <b id="selTxt" style="color:gold">-</b><br>Total: <b id="totTxt" style="color:gold">$0</b></p></div>
<div class="card"><input id="nom" placeholder="NOMBRE COMPLETO"><input id="tel" placeholder="WHATSAPP 09..."><input id="ciu" placeholder="CIUDAD"><button class="btn" onclick="irAPago()">GUARDAR Y PAGAR →</button></div>
</div>

<div id="p3">
<button onclick="irANumeros()" style="background:#222;color:#fff;border:1px solid #444;border-radius:8px;padding:8px 12px;margin-bottom:10px">← VOLVER</button>
<h2 style="text-align:center;color:gold">💳 PAGA TU RESERVA</h2>
<div class="card" style="text-align:center"><p id="resNums" style="color:gold;font-weight:900"></p><p id="resTot" style="font-size:22px;font-weight:900"></p></div>
<div class="pagoBox"><b>🏦 PICHINCHA - Cuenta Ahorros: 2201234567</b><br>Nombre: Jorge R. - CI: 0912345678<br><button class="btn" style="padding:10px;margin-top:8px" onclick="navigator.clipboard.writeText('2201234567');alert('Copiado')">COPIAR CUENTA</button></div>
<div class="pagoBox"><b>🏦 GUAYAQUIL - Cuenta: 0012345678</b><br><button class="btn" style="padding:10px;margin-top:8px;background:#fff" onclick="navigator.clipboard.writeText('0012345678');alert('Copiado')">COPIAR</button></div>
<button class="btn" style="background:#25D366;color:#fff;margin-top:12px" onclick="enviarWhats()">📲 ENVIAR COMPROBANTE WHATSAPP</button>
</div>

</div>
<script>
let sel=[],vend=JSON.parse(localStorage.getItem('thewin_final')||'{}'),datos={};
const grid=document.getElementById('grid');
for(let i=1;i<=1000;i++){let d=document.createElement('div');d.className='num';d.innerText=String(i).padStart(4,'0');d.dataset.n=i;if(vend[i])d.classList.add('vend');d.onclick=()=>{if(d.classList.contains('vend'))return;let n=+d.dataset.n;if(sel.includes(n)){sel=sel.filter(x=>x!==n);d.classList.remove('sel')}else{if(sel.length>=20)return;sel.push(n);d.classList.add('sel')}upd()};grid.appendChild(d);}
function upd(){sel.sort((a,b)=>a-b);document.getElementById('selTxt').innerText=sel.length?sel.map(x=>String(x).padStart(4,'0')).join(', '):'-';document.getElementById('totTxt').innerText='$'+sel.length;let c=Object.keys(vend).length;document.getElementById('vend1').innerText=c;document.getElementById('vend2').innerText=c;document.getElementById('fill1').style.width=(c/10)+'%';document.getElementById('porc1').innerText=c/10+'% VENDIDO ('+c+'/1000)';}
upd();
function irAPrincipal(){document.getElementById('pantalla1').style.display='block';document.getElementById('p2').style.display='none';document.getElementById('p3').style.display='none';}
function irANumeros(){document.getElementById('pantalla1').style.display='none';document.getElementById('p2').style.display='block';document.getElementById('p3').style.display='none';window.scrollTo(0,0);}
function autoSel(){sel=[];document.querySelectorAll('.num').forEach(e=>e.classList.remove('sel'));let disp=[];for(let i=1;i<=1000;i++)if(!vend[i])disp.push(i);for(let k=0;k<5&&disp.length;k++){let idx=Math.floor(Math.random()*disp.length);let n=disp.splice(idx,1)[0];sel.push(n);document.querySelector(`.num[data-n="${n}"]`)?.classList.add('sel')}upd()}
function irAPago(){if(sel.length<5){alert('Minimo 5');return}let nom=document.getElementById('nom').value.trim();let tel=document.getElementById('tel').value.replace(/\D/g,'');if(!nom||tel.length<9){alert('Nombre y WhatsApp');return}datos={nom,tel,nums:[...sel],total:sel.length,ciu:document.getElementById('ciu').value};sel.forEach(n=>vend[n]={nom,tel});localStorage.setItem('thewin_final',JSON.stringify(vend));document.getElementById('resNums').innerText='Numeros: '+sel.map(x=>String(x).padStart(4,'0')).join(', ');document.getElementById('resTot').innerText='TOTAL: $'+sel.length+',00';document.getElementById('pantalla1').style.display='none';document.getElementById('p2').style.display='none';document.getElementById('p3').style.display='block';window.scrollTo(0,0);}
function enviarWhats(){let txt=datos.nums.map(n=>String(n).padStart(4,'0')).join(', ');let msg=`Hola THE WIN! Mis numeros: ${txt} Total $${datos.total} Nombre ${datos.nom}`;window.open(`https://wa.me/593${datos.tel.slice(-9)}?text=${encodeURIComponent(msg)}`,'_blank');}
irAPrincipal();
</script></body></html>
