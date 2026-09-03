html<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>THE WIN - RIFA OFICIAL</title>
<style>
*{box-sizing:border-box}body{margin:0;background:#000;color:#fff;font-family:Arial,sans-serif}.wrap{max-width:480px;margin:auto;padding:12px}
.card{border:1px solid #C5A028;border-radius:16px;background:#111;padding:16px;margin:12px 0}
.bar{background:#222;height:30px;border-radius:20px;overflow:hidden;position:relative}.fill{height:100%;background:linear-gradient(90deg,#C5A028,#F9E27D);width:0%;transition:0.5s}
.grid{display:grid;grid-template-columns:repeat(8,1fr);gap:5px;max-height:350px;overflow-y:auto;background:#0a0a0a;padding:10px;border-radius:12px;border:1px solid #222}
.num{border:1px solid #C5A028;height:38px;display:flex;align-items:center;justify-content:center;font-size:10px;font-weight:800;background:#1a1a1a;border-radius:8px;cursor:pointer;user-select:none}.num.sel{background:#C5A028;color:#000}.num.vend{background:#3a0000;color:#555;border-color:#500;text-decoration:line-through;cursor:not-allowed}
.btn{width:100%;padding:18px;border:none;border-radius:14px;font-weight:900;background:linear-gradient(90deg,#C5A028,#F9E27D);color:#000;font-size:17px;cursor:pointer}input{width:100%;padding:14px;margin:7px 0;border-radius:10px;border:1px solid #333;background:#1a1a1a;color:#fff;font-size:15px}
.hidden{display:none}
</style>
</head>
<body>
<div class="wrap">

<!-- ================= PANTALLA 1 : PRINCIPAL ================= -->
<div id="screen1">
<div style="text-align:center;padding:15px 0"><div style="width:80px;height:80px;margin:0 auto;border-radius:50%;background:linear-gradient(135deg,#C5A028,#F9E27D);display:flex;align-items:center;justify-content:center;color:#000;font-weight:900">THE WIN</div><h1 style="color:#C5A028;margin:10px 0 0">GRAN SORTEO</h1><h2 style="margin:0">KEEWAY MINNIX 150</h2></div>

<div class="card"><h3 style="color:gold;text-align:center;margin-top:0">🏆 PREMIOS</h3><p>🏍️ 1er: Moto Keeway 150 0km</p><p>📱 2do: iPhone</p><p>⛑️ 3er: Casco Certificado</p></div>

<div class="card"><div style="display:flex;justify-content:space-between"><b>PROGRESO</b><b style="color:gold"><span id="vendidos1">0</span>/1000</b></div><div class="bar" style="margin-top:10px"><div class="fill" id="fill1"></div></div><p id="porcTxt" style="text-align:center;margin:8px 0 0">0% VENDIDO</p></div>

<div class="card" style="text-align:center"><p>VALOR POR NUMERO</p><p style="font-size:45px;font-weight:900;color:gold;margin:0">$1.00</p><p style="font-size:12px;color:#aaa">Mínimo 5 números</p><hr style="border-color:#222"><p>📞 CONTACTO OFICIAL</p><p style="font-size:22px;font-weight:900;color:#25D366;margin:0">099 123 4567</p></div>

<button type="button" id="btnComprar" class="btn">🎟️ COMPRAR NÚMEROS →</button>
</div>

<!-- ================= PANTALLA 2 : NUMEROS ================= -->
<div id="screen2" class="hidden">
<button type="button" id="btnVolver1" style="background:#222;color:#fff;border:1px solid #444;padding:10px 15px;border-radius:8px">← VOLVER</button>
<h2 style="text-align:center;color:gold">ELIGE TUS NÚMEROS</h2>
<div class="card"><div style="display:flex;justify-content:space-between;align-items:center"><span>Vendidos: <b id="vendidos2">0</b>/1000</span><button type="button" id="btnRandom" style="background:#222;color:gold;border:1px solid gold;padding:5px 10px;border-radius:6px">🎲 5 Aleatorios</button></div><div class="grid" id="gridNumeros"></div><p style="text-align:center">Seleccionados: <b id="txtSel" style="color:gold">-</b><br>Total: <b id="txtTot" style="color:gold">$0</b></p></div>
<div class="card"><input id="nombre" placeholder="NOMBRE COMPLETO"><input id="whatsapp" placeholder="WHATSAPP 09xxxxxxxx"><input id="ciudad" placeholder="CIUDAD"><button type="button" id="btnPagar" class="btn">GUARDAR Y VER CUENTAS →</button></div>
</div>

<!-- ================= PANTALLA 3 : PAGOS ================= -->
<div id="screen3" class="hidden">
<button type="button" id="btnVolver2" style="background:#222;color:#fff;border:1px solid #444;padding:10px 15px;border-radius:8px">← CAMBIAR NÚMEROS</button>
<h2 style="text-align:center;color:gold">💳 MÉTODOS DE PAGO</h2>
<div class="card" style="text-align:center;border:2px solid gold"><p id="resumenNums" style="font-weight:900;color:gold;font-size:16px"></p><p id="resumenTotal" style="font-size:24px;font-weight:900"></p></div>
<div class="card" style="border:2px solid gold"><h3 style="margin-top:0">🏦 BANCO PICHINCHA</h3><p><b>Cuenta Ahorros:</b> 2201234567<br><b>A Nombre:</b> Jorge R.<br><b>CI:</b> 0912345678</p><button type="button" class="btn" style="padding:12px" onclick="navigator.clipboard.writeText('2201234567');alert('Cuenta copiada: 2201234567')">COPIAR CUENTA PICHINCHA</button></div>
<div class="card"><h3 style="margin-top:0">🏦 BANCO GUAYAQUIL</h3><p><b>Cuenta:</b> 0012345678</p><button type="button" class="btn" style="padding:12px;background:#fff" onclick="navigator.clipboard.writeText('0012345678');alert('Cuenta copiada')">COPIAR CUENTA GUAYAQUIL</button></div>
<div class="card"><h3 style="margin-top:0">📱 DEUNA</h3><p><b>Número:</b> 0991234567</p></div>
<button type="button" id="btnWhatsapp" class="btn" style="background:#25D366;color:#fff">📲 ENVIAR COMPROBANTE POR WHATSAPP</button>
</div>

</div>

<script>
// VARIABLES GLOBALES
let seleccionados = [];
let vendidos = JSON.parse(localStorage.getItem('thewin_final_v5') || '{}');
let datosCliente = {};

// CREAR GRID 1-1000
const grid = document.getElementById('gridNumeros');
for(let i=1; i<=1000; i++){
  let div = document.createElement('div');
  div.className = 'num';
  div.textContent = String(i).padStart(4,'0');
  div.dataset.numero = i;
  if(vendidos[i]){ div.classList.add('vend'); }
  div.addEventListener('click', function(){
    if(this.classList.contains('vend')) return;
    let n = parseInt(this.dataset.numero);
    if(seleccionados.includes(n)){
      seleccionados = seleccionados.filter(x => x!== n);
      this.classList.remove('sel');
    } else {
      if(seleccionados.length >= 20){ alert('Máximo 20 números'); return; }
      seleccionados.push(n);
      this.classList.add('sel');
    }
    actualizarUI();
  });
  grid.appendChild(div);
}

function actualizarUI(){
  seleccionados.sort((a,b)=>a-b);
  document.getElementById('txtSel').textContent = seleccionados.length? seleccionados.map(n=>String(n).padStart(4,'0')).join(', ') : '-';
  document.getElementById('txtTot').textContent = '$' + seleccionados.length + '.00';
  let totalVendidos = Object.keys(vendidos).length;
  document.getElementById('vendidos1').textContent = totalVendidos;
  document.getElementById('vendidos2').textContent = totalVendidos;
  document.getElementById('fill1').style.width = (totalVendidos/10) + '%';
  document.getElementById('porcTxt').textContent = (totalVendidos/10).toFixed(1) + '% VENDIDO';
}
actualizarUI();

// BOTONES DE NAVEGACION - CON addEventListener (no falla)
document.getElementById('btnComprar').addEventListener('click', function(){
  document.getElementById('screen1').classList.add('hidden');
  document.getElementById('screen2').classList.remove('hidden');
  window.scrollTo(0,0);
});
document.getElementById('btnVolver1').addEventListener('click', function(){
  document.getElementById('screen2').classList.add('hidden');
  document.getElementById('screen1').classList.remove('hidden');
});
document.getElementById('btnVolver2').addEventListener('click', function(){
  document.getElementById('screen3').classList.add('hidden');
  document.getElementById('screen2').classList.remove('hidden');
});
document.getElementById('btnRandom').addEventListener('click', function(){
  seleccionados = [];
  document.querySelectorAll('.num').forEach(e=>e.classList.remove('sel'));
  let libres = [];
  for(let i=1;i<=1000;i++) if(!vendidos[i]) libres.push(i);
  for(let k=0;k<5 && libres.length>0;k++){
    let idx = Math.floor(Math.random()*libres.length);
    let n = libres.splice(idx,1)[0];
    seleccionados.push(n);
    document.querySelector(`.num[data-numero="${n}"]`).classList.add('sel');
  }
  actualizarUI();
});
document.getElementById('btnPagar').addEventListener('click', function(){
  if(seleccionados.length < 5){ alert('Debes elegir mínimo 5 números'); return; }
  let nom = document.getElementById('nombre').value.trim();
  let tel = document.getElementById('whatsapp').value.replace(/\D/g,'');
  let ciu = document.getElementById('ciudad').value.trim();
  if(nom.length < 3){ alert('Escribe tu nombre completo'); return; }
  if(tel.length < 9){ alert('Escribe tu WhatsApp válido'); return; }
  datosCliente = {nombre:nom, telefono:tel, ciudad:ciu, numeros:[...seleccionados], total:seleccionados.length};
  seleccionados.forEach(n=>vendidos[n]={nombre:nom, tel:tel, fecha:Date.now()});
  localStorage.setItem('thewin_final_v5', JSON.stringify(vendidos));
  document.getElementById('resumenNums').textContent = 'NÚMEROS: ' + datosCliente.numeros.map(n=>String(n).padStart(4,'0')).join(', ');
  document.getElementById('resumenTotal').textContent = 'TOTAL A PAGAR: $' + datosCliente.total + '.00';
  document.getElementById('screen2').classList.add('hidden');
  document.getElementById('screen3').classList.remove('hidden');
  window.scrollTo(0,0);
});
document.getElementById('btnWhatsapp').addEventListener('click', function(){
  let nums = datosCliente.numeros.map(n=>String(n).padStart(4,'0')).join(', ');
  let mensaje = `Hola THE WIN! 🎉 Reserve mis numeros: ${nums} Total $${datosCliente.total} Nombre: ${datosCliente.nombre} Ciudad: ${datosCliente.ciudad}`;
  window.open('https://wa.me/593' + datosCliente.telefono.slice(-9) + '?text=' + encodeURIComponent(mensaje), '_blank');
});
</script>
</body>
</html>
