1-
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Perfil</title>
  <style>
    .in-box {
        margin-top: 90px;
        padding: 20px;
        border: 1px solid #ccc;
        border-radius: 10px; 
        max-width: 1000px; 
        margin-left: 190px;
        text-align: center; 
        box-shadow: 0 5px 20px rgba(0,0,0,0.3);
    }
    .perfil {
        display: flex;
        justify-content: center;
        align-items: center;
        margin: 20px 0;
    }
    .icone-perfil {
        width: 100px; 
        height: 100px; 
        background-color: #4CAF50; 
        border-radius: 50%; 
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .icone-perfil:before {
        content: "👹"; 
        font-size: 50px; 
    }
    .button-link {
        display: inline-block;
        background-color: #4fa152; 
        color: white; 
        padding: 10px 20px; 
        text-align: center; 
        text-decoration: none; 
        border-radius: 5px; 
        transition: background-color 0.3s; 
    }
    .button-link:hover {
        background-color: #45a049; /* Cor ao passar o mouse */
    }
    h2 {
        font-size: 40px;
        color: rgb(141, 212, 69);
    }
    h4 {
        font-size: 25px;
    }
    h5 {
        font-size: 14px;
    }
    a {
        color: #6da32e; 
    }
  </style>
</head>
<body>

  <div class="in-box">
    <div class="perfil">
        <div class="icone-perfil"></div>
    </div>
    <h2>Victor Yuri</h2>
    <h4>Desenvolvedor Web</h4>
    <h5>Sou um desenvolvedor web capaz de criar experiências digitais envolventes e funcionais. Com uma sólida compreensão de HTML, CSS e JavaScript, busco sempre me manter atualizado com as melhores práticas e novas tecnologias.</h5>
    <a href="#" class="button-link">HTML</a>
    <a href="#" class="button-link">CSS</a>
    <a href="#" class="button-link">JAVASCRIPT</a>
    <p>
        <a href="https://br.linkedin.com/" target="_blank">LinkedIn</a> 
        <a href="https://github.com/V1CTOR022" target="_blank">GitHub</a> 
    </p>
  </div>

</body>
</html>



2-
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tabela de Produtos</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }

        table {
            width: 100%;
            border-collapse: collapse;
        }

        th, td {
            padding: 10px;
            text-align: left;
            border: 1px solid #dddddd;
        }

        th {
            background-color: #4CAF50;
            color: white;
        }

        tbody tr:nth-child(even) {
            background-color: #f2f2f2; 
        }

        tbody tr:nth-child(odd) {
            background-color: #ffffff; 
        }

        tbody tr:hover {
            background-color: #d1e7dd; 
        }
    </style>
</head>
<body>
    <h1>Tabela de Produtos</h1>
    <table>
        <thead>
            <tr>
                <th>Nome</th>
                <th>Preço</th>
                <th>Categoria</th>
                <th>Descrição</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Placa Mãe</td>
                <td>R$ 999,00</td>
                <td>Eletrônicos</td>
                <td>B 550M prime</td>
            </tr>
            <tr>
                <td>Processador</td>
                <td>R$ 2034,00</td>
                <td>Eletrônicos</td>
                <td>Ryzen 4 3400 GE</td>
            </tr>
            <tr>
                <td>Monitor</td>
                <td>R$ 1567,00</td>
                <td>Eletrônicos</td>
                <td>Samsung 4K</td>
            </tr>
        </tbody>
    </table>
</body>
</html>


3-
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Formulário</title>
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body, html {
      height: 100%;
      background: rgb(255, 255, 255); 
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .formulario-box {
      background: white;
      padding: 40px;
      border-radius: 20px;
      box-shadow: 0 5px 20px rgba(0,0,0,0.3);
      width: 320px;
      text-align: center;
    }

    .formulario-box h2 {
      margin-bottom: 30px;
      color: #333;
    }

    .formulario-box input[type="text"],
    .formulario-box input[type="email"] {
      width: 100%;
      padding: 12px;
      margin-bottom: 20px;
      border: 1px solid #ccc;
      border-radius: 5px;
    }

    .formulario-box button {
      width: 100%;
      padding: 12px;
      background: #2575fc;
      border: none;
      color: white;
      font-size: 16px;
      border-radius: 5px;
      cursor: pointer;
      transition: 0.3s;
    }

    .formulario-box button:hover {
      background: #1a5fd1;
    }

    .formulario-box label {
      display: block;
      text-align: left;
      margin-bottom: 5px;
      font-weight: bold;
    }
  </style>
</head>
<body>

  <div class="formulario-box">
    <h2>Formulário de Contato</h2>
    <form>
      <label for="usuario">Nome</label>
      <input type="text" id="usuario" name="usuario" placeholder="Digite seu nome" required>

      <label for="email">Email</label>
      <input type="email" id="email" name="email" placeholder="Digite seu email" required>

      <label for="mensagem">Mensagem</label>
      <textarea id="mensagem" name="mensagem" rows="4" placeholder="Digite sua mensagem..." required></textarea>

      <button type="submit">Enviar Formulário</button>
    </form>
  </div>

</body>
</html>
