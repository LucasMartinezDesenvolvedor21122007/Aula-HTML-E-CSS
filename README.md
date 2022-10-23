<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" type="text/css" href="index.css" media="screen">
    <title>Cadastro</title>
</head>
<body>
     
    <div class="campo">
      <h1 id="Titulo">Cadastro De DEVs</h1>
      <p id="Subtitulo">Complete suas informações</p>
      <br>
    </div class="campo">

    <form>
       <fieldset class="Grupo">
            <div class="campo">
                <label for="nome"><strong>Nome</strong></label>
                <input type="text" name="Nome" id="Nome" required>
            </div class="campo">

            <div class="campo">
                <label for="Sobrenome"><strong>Sobrenome</strong></label >
                <input type="text" name="Sobrenome" id="Sobrenome" required>
            </div class="campo">
       </fieldset class="Grupo">

            <div class="campo">
                <label for="email"><strong>email</strong></label>
                <input type="email" name="email" id="email" required>
            </div class="campo">

         <div class="campo">
            <label><strong>De Qual Lado da aplicação você desenvolve</strong></label>
            <label>
                <input type="radio" name="devweb" value="Front-End">Front-End
                <input type="radio" name="devweb" value="Back-End" checked>Back-End
                <input type="radio" name="devweb" value="Fullstack">Fullstack
            </label>
         </div class="campo">

         <div class="campo">
            <label for="senioridade"><strong>senioridade</strong></label>
            <select id="senioridade">
                <option selected disabled value="">Escolha</option>
                <option>Junior</option>
                <option>Pleno</option>
                <option>Sênior</option>
            </select>
         </div class="campo">

         <fieldset class="grupo">
            <div id="check">
                <label><strong>Selecione as tecnologias que utliza:</strong></label><br><br>
                <input type="checkbox" id="tecnologia1" name="tecnologia1" value="HTML">
                <label for="tecnologia1">HTML</label>
                <input type="checkbox" id="tecnologia2" name="tecnologia2" value="CSS">
                <label for="tecnologia2">CSS</label>
                <input type="checkbox" id="tecnologia3" name="tecnologia3" value="Javascript">
                <label for="tecnologia3">Javascript</label>
                <input type="checkbox" id="tecnologia4" name="tecnologia4" value="PHP">
                <label for="tecnologia4">PHP</label>
                <input type="checkbox" id="tecnologia5" name="tecnologia5" value="C#">
                <label for="tecnologia5">C#</label>
                <input type="checkbox" id="tecnologia6" name="tecnologia6" value="Python">
                <label for="tecnologia6">Python</label>
                <input type="checkbox" id="tecnologia7" name="tecnologia7" value="Java">
                <label for="tecnologia7">Java</label>
            </div class="campo">
         </fieldset class="Grupo">

         <div class="campo">
            <br>
            <label><strong>Conte Um Pouco Da Sua Experiência</strong></label>
            <textarea row="6" style="width:26em" id="experiência" name="experiência"></textarea>
         </div class="campo">

         <button class="Botão" type="submit">Concluido!!!</button>

    </form>

*{
   Margin:0;
   padding: 0; 
}

#titulo{
    font-family:sans-serif;
    color: #380b61;
    margin-left: 10%;
}

#subtitulo{
    font-family:sans-serif;
    color: #380b61;
    margin-left: 10%;
}

fieldset{
    border:0;
}

body{
    background-color:#F0F8FF;
    font-family: sans-serif;
    font-size: 1em;
    color:#59429d;
    margin-left: 16%;
    margin-top: 3%;
    justify-content: center;
}

input, select,textarea, button{
    border-radius: 7px;
}

.campo{
    margin-bottom: 1em;
}

.campo label{
   margin-bottom: 1.2em;
   color: #59429d;
   display: inline-block;
}

fieldset.grupo.campo{
    float: left;
    margin-right: 1em;
}

.campo input [type="text"], .campo input[type="email"], .campo select, .campo textarea{
    padding:0.2em; 
    border:1px solid #59429d;
    box-shadow: 2px, 2px, 2px rgb(0,0,0,0.2);
    display:block;
}

.campo select, option{
    padding-right: 1em;
}

.campo input:focus, .campo select:focus, .campo textarea:focus{
    background-color: #e0e0f8;
}

.botão {
    font-size: 1.2em;
    background: #59429d;
    border:0;
    margin-bottom: 1em;
    color:#ffffff;
    padding: 0.2em 0.6em;
    box-shadow: 2px 2px 2px rgba(0,0,0.2);
    text-shadow:  1px, 1px, 1px, 1px rgba(0,0,0,0.5);
    position:absolute;
    top:90%;
    left:50%;
    margin-right:-50%;
    transform:translate(-50%, -50%)
}

.botão:hover {
    background: #ccbbff;
    box-shadow: inset 2px 2px 2px rgba(0,0,0,0.2);
    text-shadow:none;
}

#check{
    display: inline-block;
}

</body>
</html>
