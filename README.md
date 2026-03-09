<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TuRadar
  Inmobiliario</title>
  <style>
        body { background-color: #000; color: white; font-family: 'Segoe UI', sans-serif; padding: 15px; text-align: center; }
        .card { 
    background: linear-gradient(135deg, rgba(20, 20, 20, 0.9), rgba(0, 0, 0, 0.95));
    backdrop-filter: blur(10px);
    padding: 20px; 
    border-radius: 20px; 
    border: 1px solid #00ff88; /* El verdecito tecnológico */
    width: 90%; 
    max-width: 400px; 
    margin: 20px auto; 
    box-shadow: 0 0 15px rgba(0, 255, 136, 0.2); /* Resplandor verde sutil */
    text-align: left;
}
        .input-radar { width: 95%; padding: 12px; margin-bottom: 12px; border-radius: 8px; border: 1px solid #444; background: #000; color: #ff6600; text-align: center; font-size: 15px; font-weight: bold; }
        .btn-naranja { background: linear-gradient(45deg, #ff6600, #ffbb00); color: black; padding: 18px; border: none; border-radius: 12px; font-weight: bold; cursor: pointer; width: 100%; font-size: 17px; text-transform: uppercase; }
        #confetti-container { position: fixed; top: 0; left: 0; width: 100%; height: 100%; pointer-events: none; z-index: 9999; }
        
        /* Estilo del Termómetro */
        .termo-container { display: flex; justify-content: space-around; align-items: flex-end; background: #111; padding: 15px; border-radius: 20px; height: 180px; margin-bottom: 20px; border: 1px solid #444; position: relative; }
        <div style="margin-top: 25px; text-align: center;">
    <p style="color: #00ff88; font-weight: bold; letter-spacing: 1px;">📸 CARGA DE ACTIVOS</p>
    
    <label class="btn-radar-verde" style="display: block; background: rgba(0,255,136,0.1); border: 1px solid #00ff88; color: white; padding: 12px; margin-bottom: 10px; border-radius: 10px; cursor: pointer;">
        CAPTURA FACHADA
        <input type="file" accept="image/*" capture="environment" style="display: none;">
    </label></div>

    <label class="btn-radar-verde" style="display: block; background: rgba(0,255,136,0.1); border: 1px solid #00ff88; color: white; padding: 12px; margin-bottom: 10px; border-radius: 10px; cursor: pointer;">
        CAPTURA SALA
        <input type="file" accept="image/*" capture="environment" style="display: none;">
    </label></div>

    <label class="btn-radar-verde" style="display: block; background: rgba(0,255,136,0.1); border: 1px solid #00ff88; color: white; padding: 12px; border-radius: 10px; cursor: pointer;">
        CAPTURA COCINA
        <input type="file" accept="image/*" capture="environment" style="display: none;">
    </label>
</div>

    </style>
</head>
<body> <div style="text-align: center; margin-top: 15px;">
    <img src="logo tuRadar inmobiliario.png" alt="TuRadar Inmobiliario" style="width: 180px; filter: drop-shadow(0px 0px 8px #ff6600);">
    
    <h1 style="color: #ff6600; font-family: sans-serif; margin: 10px 0 5px 0; letter-spacing: 2px; text-transform: uppercase; font-size: 24px;">
        TURADAR INMOBILIARIO
    </h1>
    <p style="color: #666; font-size: 10px; letter-spacing: 4px; font-weight: bold; margin-bottom: 20px;">
        SISTEMA DE CAPTACIÓN INTELIGENTE
    </p>
</div>
<div style="margin-bottom: 20px;">
    <p style="color: #00ff88; font-weight: bold;">BAÑO</p>
    <label class="btn-radar-verde" style="display: block;">
        CAPTURA BAÑO
        <input type="file" accept="image/*" capture="environment" style="display:none;">
    </label>
</div>
<div style="margin-bottom: 20px;">
    <p style="color: #00ff88; font-weight: bold;">EXTRAS / PATIO / OTROS</p>
    <label class="btn-radar-verde" style="display: block;">
        CAPTURA EXTRAS
        <input type="file" accept="image/*" capture="environment" style="display:none;">
    </label>
</div>

 <div style="margin-bottom: 20px;">
    <p style="color: #00ff88; font-weight: bold;">HABITACIÓN</p>
    <label class="btn-radar-verde" style="display: block;">
        CAPTURA HABITACIÓN
        <input type="file" accept="image/*" capture="environment" style="none">
    </label>
</div>   
    
<div style="background: #111; padding: 15px; border-radius: 15px; border-left: 5px solid #00ff88; margin-bottom: 15px;">
    <p style="color: #00ff88; font-size: 11px; font-weight: bold; margin-bottom: 10px; letter-spacing: 1px;">ESTADO DE IMPUESTOS Y SERVICIOS</p>
    
    <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 8px;">
        <label style="display: flex; align-items: center; background: #1a1a1a; padding: 10px; border-radius: 8px; border: 1px solid #333; cursor: pointer;">
            <input type="checkbox" style="margin-right: 8px; accent-color: #00ff88;">
            <span style="color: #fff; font-size: 11px;">Derecho de Frente</span>
        </label>

        <label style="display: flex; align-items: center; background: #1a1a1a; padding: 10px; border-radius: 8px; border: 1px solid #333; cursor: pointer;">
            <input type="checkbox" style="margin-right: 8px; accent-color: #00ff88;">
            <span style="color: #fff; font-size: 11px;">Ficha Catastral</span>
        </label>

        <label style="display: flex; align-items: center; background: #1a1a1a; padding: 10px; border-radius: 8px; border: 1px solid #333; cursor: pointer;">
            <input type="checkbox" style="margin-right: 8px; accent-color: #00ff88;">
            <span style="color: #fff; font-size: 11px;">Solvencia Aseo</span>
        </label>

        <label style="display: flex; align-items: center; background: #1a1a1a; padding: 10px; border-radius: 8px; border: 1px solid #333; cursor: pointer;">
            <input type="checkbox" style="margin-right: 8px; accent-color: #00ff88;">
            <span style="color: #fff; font-size: 11px;">Luz / Agua</span>
        </label>
    </div>
</div>
    <div style="text-align: right; margin-bottom: 10px;">
<div style="background: linear-gradient(180deg, #0a0a0a 0%, #111111 100%); padding: 25px; border-radius: 20px; border: 1px solid rgba(255,255,255,0.1); margin-top: 20px; font-family: sans-serif; box-shadow: 0 10px 30px rgba(0,0,0,0.5);">
    
    <p style="color: #ffffff; font-weight: 900; text-align: center; margin-bottom: 25px; letter-spacing: 2px; text-transform: uppercase; font-size: 14px;">
        Auditoría Técnica Legal
    </p>

    <div style="display: flex; gap: 12px; margin-bottom: 20px;">
        <div style="flex: 1;">
            <label style="color: #888; font-size: 10px; font-weight: 800; display: block; margin-bottom: 8px;">ANCHO (MTS)</label>
            <input type="number" placeholder="0.00" style="width: 100%; padding: 15px; background: #000; color: #ffffff; border: 1px solid #333; border-radius: 12px; font-weight: bold;">
        </div>
        <div style="flex: 1;">
            <label style="color: #888; font-size: 10px; font-weight: 800; display: block; margin-bottom: 8px;">LARGO (MTS)</label>
            <input type="number" placeholder="0.00" style="width: 100%; padding: 15px; background: #000; color: #ffffff; border: 1px solid #333; border-radius: 12px; font-weight: bold;">
        </div>
    </div>

    <div style="background: rgba(255,255,255,0.03); padding: 18px; border-radius: 15px; border: 1px solid #222; margin-bottom: 20px;">
        <p style="color: #ffffff; font-size: 10px; font-weight: 900; margin-bottom: 15px; text-transform: uppercase;">Solvencias Confirmadas</p>
        <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 15px;">
            <label style="color: #ffffff; font-size: 13px; font-weight: 600; display: flex; align-items: center;">
                <input type="checkbox" style="margin-right: 10px;"> Derecho de Frente
            </label>
            <label style="color: #ffffff; font-size: 13px; font-weight: 600; display: flex; align-items: center;">
                <input type="checkbox" style="margin-right: 10px;"> Ficha Catastral
            </label>
        </div>
    </div>

    <button style="width: 100%; background: #ffffff; color: #000000; font-weight: 900; padding: 20px; border: none; border-radius: 15px; font-size: 14px; text-transform: uppercase; letter-spacing: 2px;">
        Firmar Acuerdo Gestión (5%)
    </button>
</div>
        <span style="color: #ff6600; font-family: monospace; font-weight: bold; background: #222; padding: 5px 12px; border-radius: 5px; border: 1px solid #ff6600;">
            CONTROL N°: <span id="num-folio">0000</span>
        </span>
    </div><div id="termometro-container" style="width: 100%; background: #222; border-radius: 10px; padding: 5px; margin: 5px 0 10px 0; border: 1px solid #444;">
    <div id="merc-indiv" style="width: 0%; height: 25px; background: linear-gradient(90deg, #ff6600, #ffbb00); border-radius: 8px; transition: width 2s ease-in-out; display: flex; align-items: center; justify-content: center;">
        <span id="porcentaje-texto" style="color: black; font-weight: bold; font-family: sans-serif; font-size: 12px;">0%</span>
    </div>
</div>
<p style="text-align: center; color: #ff6600; font-size: 10px; font-weight: bold; margin: -5px 0 15px 0;">PROGRESO DE CAPTACIÓN INTELIGENTE</p>
</div>
<p style="text-align: center; color: #ff8c00; font-family: sans-serif; font-size

    <div class="termo-container">
        <div style="display: flex; flex-direction: column; align-items: center;">
            <span style="font-size: 20px;">🏆</span>
            <div style="width: 25px; height: 120px; background: #222; border-radius: 12px; border: 2px solid #ff6600; overflow: hidden; display: flex; flex-direction: column-reverse;">
                <div id="merc-grupal" class="mercurio" style="height: 10%;"></div>
            </div>
            <p style="color: #ff6600; font-size: 10px; font-weight: bold; margin-top: 5px;">EQUIPO (200)</p>
        </div>
        
        <div style="display: flex; flex-direction: column; align-items: center;">
            <span id="icono-regalo" style="font-size: 20px; filter: grayscale(1);">🎁</span>
            <div style="width: 18px; height: 100px; background: #222; border-radius: 10px; border: 2px solid #00ff00; overflow: hidden; display: flex; flex-direction: column-reverse;">
                <div id="merc-indiv" class="mercurio-v" style="height: 10%;"></div>
            </div>
            <p style="color: #00ff00; font-size: 10px; font-weight: bold; margin-top: 5px;">TU RETO (50)</p>
        </div>
        <div style="position: absolute; top: 10px; right: 15px; color: #fff; font-size: 18px; font-weight: bold;" id="txt-grupal">0/200</div>
    </div>

    <div class="card">
        <p style="color: #ff6600; font-weight: bold; margin: 0 0 12px 0; border-bottom: 1px solid #333; padding-bottom: 5px;">👨‍💼 VALIDACIÓN DE AGENTE</p>
        <input type="text" id="agente-nom" placeholder="Escribe tu Nombre" class="input-radar">
        <input type="number" id="agente-ci" placeholder="Tu Cédula" class="input-radar">
        <input type="file" accept="image/*" capture="user" id="selfie-file" style="display: none;">
        <button onclick="document.getElementById('selfie-file').click()" style="background: #333; color: white; border: 1px solid #ff6600; padding: 10px; width: 100%; border-radius: 8px; cursor: pointer; font-weight: bold;">📸 TOMAR SELFIE DE ENTRADA</button>
        <div id="status-selfie" style="display:none; color:#00ff00; font-size:12px; margin-top:8px; text-align:center;">✅ Identidad Verificada</div>
    </div>

    <div class="card">
        <p style="color: #ff6600; font-weight: bold; margin: 0 0 12px 0; border-bottom: 1px solid #333; padding-bottom: 5px;">🏠 DATOS DEL CLIENTE</p>
        <input type="text" id="prop-nom" placeholder="Nombre del Propietario" class="input-radar">
        <input type="number" id="prop-tel" placeholder="WhatsApp del Cliente" class="input-radar">
        
        <p style="color: #ccc; font-size: 12px; margin-bottom: 5px;">Estatus del Pago:</p>
        <select id="pago-status" onchange="mostrarFecha()" class="input-radar" style="width: 100%; height: 45px; background: #000;">
            <option value="pagado">✅ PAGADO AHORA</option>
            <option value="pendiente">📅 PAGO PENDIENTE (ALMANAQUE)</option>
        </select>

        <div id="almanaque-box" style="display: none; margin-top: 15px; border-top: 1px dashed #444; padding-top: 10px;">
            <p style="color: #ffcc00; font-size: 12px; font-weight: bold;">📆 ¿QUÉ DÍA PAGARÁ?</p>
            <input type="date" id="fecha-compromiso" class="input-radar">
        </div>
    </div>

    <button onclick="enviarFinal()" class="btn-naranja">🚀 FINALIZAR Y NOTIFICAR</button>

    <div id="confetti-container"></div>

    <script>
        // Generar folio al azar por ahora
        document.getElementById('num-folio').innerText = Math.floor(Math.random()*9000) + 1000;

        function mostrarFecha() {
            var val = document.getElementById('pago-status').value;
            document.getElementById('almanaque-box').style.display = (val === 'pendiente') ? 'block' : 'none';
        }

        document.getElementById('selfie-file').onchange = function() {
            if(this.files.length > 0) document.getElementById('status-selfie').style.display = 'block';
        };

        function lanzarConfeti() {
            const container = document.getElementById('confetti-container');
            const emojis = ['🎉', '💰', '🏠', '🔥', '✨'];
            for (let i = 0; i < 60; i++) {
                const div = document.createElement('div');
                div.innerText = emojis[Math.floor(Math.random() * emojis.length)];
                div.style.position = 'absolute';
                div.style.left = Math.random() * 100 + 'vw';
                div.style.top = '-50px';
                div.style.fontSize = '30px';
                div.style.transition = 'transform 3s linear, opacity 3s';
                container.appendChild(div);
                setTimeout(() => {
                    div.style.transform = `translateY(110vh) rotate(${Math.random() * 360}deg)`;
                    div.style.opacity = '0';
                }, 100);
            }
        }

        function enviarFinal() {
            const prop = document.getElementById('prop-nom').value;
            const tel = document.getElementById('prop-tel').value;
            const status = document.getElementById('pago-status').value;
            const fecha = document.getElementById('fecha-compromiso').value;
            const folio = document.getElementById('num-folio').innerText;
            const agente = document.getElementById('agente-nom').value;

            if(!prop || !tel || !agente) {
                alert("❌ Error: Agente y Propietario son obligatorios.");
                return;
            }

            // Lógica de WhatsApp
            let texto = `¡Hola *${prop}*! Soy *${agente}* de *TuRadar Inmobiliario*.%0A%0A`;
            texto += `Hemos registrado su propiedad con el folio *N°${folio}*.%0A`;
            
            if(status === 'pagado') {
                texto += "✅ Su pago ha sido confirmado. ¡Iniciamos la publicidad!";
            } else {
                texto += `📅 Su compromiso de pago quedó para el: *${fecha}*.`;
            }

            // Simular subida de barra para el ejemplo
            document.getElementById('merc-indiv').style.height = "100%";
            document.getElementById('icono-regalo').style.filter = "grayscale(0)";
            lanzarConfeti();

            setTimeout(() => {
                window.open(`https://api.whatsapp.com/send?phone=58${tel}&text=${texto}`);
                alert("🚀 REGISTRO EXITOSO: Datos guardados y comprobante enviado.");
            }, 800);
        }
    </script>
</body>
</html>
