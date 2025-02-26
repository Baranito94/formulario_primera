<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Cuestionario de Primera Visita</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f4f4f4;
      margin: 20px;
    }
    .container {
      background: #fff;
      padding: 20px;
      max-width: 800px;
      margin: auto;
      border-radius: 8px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
    }
    h1, h2, h3 {
      text-align: center;
    }
    .form-group {
      margin-bottom: 15px;
    }
    label {
      font-weight: bold;
      display: block;
      margin-bottom: 5px;
    }
    input[type="text"],
    input[type="number"],
    textarea {
      width: 100%;
      padding: 8px;
      border: 1px solid #ccc;
      border-radius: 4px;
    }
    .inline {
      display: inline-block;
      margin-right: 15px;
    }
    button {
      background-color: #007BFF;
      color: #fff;
      border: none;
      padding: 10px 20px;
      border-radius: 4px;
      cursor: pointer;
      display: block;
      margin: 20px auto;
    }
    button:hover {
      background-color: #0056b3;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>CLÍNICA DR. RUBIO UROLOGÍA Y ANDROLOGÍA</h1>
    <h2>HOSPITAL 9 OCTUBRE VITHAS VALENCIA</h2>
    <p><strong>CUESTIONARIO DE PRIMERA VISITA</strong> (Por favor, rellene y entregue este formulario al personal antes de la consulta)</p>
    
    <form action="https://formspree.io/f/tuFormID" method="POST">
      <h3>ANAMNESIS - ANTECEDENTES</h3>
      
      <!-- Alergia a fármacos -->
      <div class="form-group">
        <label>ALERGIA A FÁRMACOS:</label>
        <div class="inline">
          <input type="radio" id="alergia_si" name="alergia" value="si" required>
          <label for="alergia_si">SÍ</label>
        </div>
        <div class="inline">
          <input type="radio" id="alergia_no" name="alergia" value="no" required>
          <label for="alergia_no">NO</label>
        </div>
      </div>
      <div class="form-group">
        <label for="alergia_detalle">EN CASO AFIRMATIVO, INDIQUE A CUÁL:</label>
        <input type="text" id="alergia_detalle" name="alergia_detalle">
      </div>
      
      <!-- Factores de riesgo cardiovascular -->
      <div class="form-group">
        <label>FACTORES DE RIESGO CARDIOVASCULAR (se considera afirmativo, aunque esté controlado con tratamiento):</label>
        <div>
          <strong>Hipertensión arterial:</strong>
          <div class="inline">
            <input type="radio" id="hta_si" name="hta" value="si" required>
            <label for="hta_si">SÍ</label>
          </div>
          <div class="inline">
            <input type="radio" id="hta_no" name="hta" value="no" required>
            <label for="hta_no">NO</label>
          </div>
        </div>
        <div>
          <strong>Diabetes:</strong>
          <div class="inline">
            <input type="radio" id="diabetes_si" name="diabetes" value="si" required>
            <label for="diabetes_si">SÍ</label>
          </div>
          <div class="inline">
            <input type="radio" id="diabetes_no" name="diabetes" value="no" required>
            <label for="diabetes_no">NO</label>
          </div>
        </div>
        <div>
          <strong>Colesterol:</strong>
          <div class="inline">
            <input type="radio" id="colesterol_si" name="colesterol" value="si" required>
            <label for="colesterol_si">SÍ</label>
          </div>
          <div class="inline">
            <input type="radio" id="colesterol_no" name="colesterol" value="no" required>
            <label for="colesterol_no">NO</label>
          </div>
        </div>
      </div>
      
      <!-- Fuma -->
      <div class="form-group">
        <label>FUMA:</label>
        <div class="inline">
          <input type="radio" id="fuma_si" name="fuma" value="si" required>
          <label for="fuma_si">SÍ</label>
        </div>
        <div class="inline">
          <input type="radio" id="fuma_no" name="fuma" value="no" required>
          <label for="fuma_no">NO</label>
        </div>
      </div>
      <div class="form-group">
        <label for="cigarrillos">En caso afirmativo: indique cuántos cigarrillos de media al día:</label>
        <input type="number" id="cigarrillos" name="cigarrillos" min="0">
      </div>
      <div class="form-group">
        <label for="años_fumar">Desde hace (años):</label>
        <input type="number" id="años_fumar" name="años_fumar" min="0">
      </div>
      
      <!-- Otros antecedentes médicos -->
      <div class="form-group">
        <label for="antecedentes_medicos">OTROS ANTECEDENTES MÉDICOS (Enfermedades que padezca o haya padecido en el pasado):</label>
        <textarea id="antecedentes_medicos" name="antecedentes_medicos" rows="4"></textarea>
      </div>
      
      <!-- Intervenciones quirúrgicas -->
      <div class="form-group">
        <label for="intervenciones">INTERVENCIONES QUIRÚRGICAS A LAS QUE SE HA SOMETIDO EN EL PASADO, CON FECHA (AÑO):</label>
        <textarea id="intervenciones" name="intervenciones" rows="4"></textarea>
      </div>
      
      <!-- Tratamiento habitual -->
      <div class="form-group">
        <label for="tratamiento">TRATAMIENTO HABITUAL QUE TOMA DIARIAMENTE DE MANERA CRÓNICA:</label>
        <textarea id="tratamiento" name="tratamiento" rows="4"></textarea>
      </div>
      
      <button type="submit">Enviar Formulario</button>
    </form>
  </div>
</body>
</html>
