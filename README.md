<Atualização>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Portal RH - Atualização Salarial</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f8f9fa;
      margin: 0;
      padding: 0;
    }
    .container {
      max-width: 400px;
      margin: 80px auto;
      padding: 30px;
      background-color: white;
      border: 1px solid #ccc;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
    h2, h3 {
      color: #d9534f;
      text-align: center;
    }
    label {
      display: block;
      margin-top: 15px;
    }
    input[type="text"],
    input[type="password"],
    input[type="number"] {
      width: 100%;
      padding: 8px;
      margin-top: 5px;
      border: 1px solid #ccc;
      border-radius: 4px;
    }
    button, a.button-link {
      margin-top: 20px;
      width: 100%;
      padding: 10px;
      background-color: #d9534f;
      border: none;
      color: white;
      font-weight: bold;
      cursor: pointer;
      border-radius: 4px;
      text-align: center;
      text-decoration: none;
      display: inline-block;
    }
    .warning {
      color: #d9534f;
      font-size: 0.9em;
      margin-top: 10px;
      text-align: center;
    }
    .img-box {
      margin-top: 20px;
      text-align: center;
    }
    .img-box img {
      max-width: 100%;
      border: 1px solid #aaa;
      margin-top: 15px;
    }
  </style>
</head>
<body>

<!-- Página principal -->
<div class="container" id="pagina1">
  <h2>Atualize seus dados salariais.
 TUPINAMBA LTDA</h2>
  <form onsubmit="mostrarMensagem(event)">
    <label for="user">Nome de usuário:</label>
    <input type="text" id="user" name="user" placeholder="Ex: carlos.silva">

    <label for="password">Senha da Intranet:</label>
    <input type="password" id="password" name="password" placeholder="Digite sua senha">

    <label for="funcionario">Número do Funcionário:</label>
    <input type="number" id="funcionario" name="funcionario" placeholder="Ex: 2025301">

    <label for="cpf">CPF:</label>
    <input type="text" id="cpf" name="cpf" placeholder="Ex: 123.456.789-00">

    <label for="rg">Identidade (RG):</label>
    <input type="text" id="rg" name="rg" placeholder="Ex: 123456789 SSP-CE">

    <button type="submit">Confirmar Atualização</button>
  </form>
  <div class="warning">
    Evite perder seus benefícios! Atualize agora.
  </div>
</div>

<!-- Página de agradecimento com imagens -->
<div class="container" id="pagina2" style="display: none;">
  <h3>Obrigado pelos dados!</h3>
  <p style="text-align: center; font-size: 1.1em;">
    Logo logo você terá retornos... 😏😈
  </p>
</div>

<script>
  function mostrarMensagem(event) {
    event.preventDefault();
    document.getElementById("pagina1").style.display = "none";
    document.getElementById("pagina2").style.display = "block";
  }
</script>

</body>
</html>
