
document.addEventListener("DOMContentLoaded", function () {
    const form = document.getElementById("formCadastro");
    const telefoneInput = document.getElementById("telefone");

    
    const msgErro = document.createElement("p");
    msgErro.className = "form-erro";
    const msgSucesso = document.createElement("p");
    msgSucesso.className = "form-sucesso";

    const botaoEnviar = form.querySelector("button");
    form.insertBefore(msgErro, botaoEnviar);
    form.insertBefore(msgSucesso, botaoEnviar);

   
    form.querySelectorAll("input, select").forEach(campo => {
        campo.addEventListener("input", () => {
            msgErro.textContent = "";
        });
    });

    
    telefoneInput.addEventListener("input", function (e) {
        let value = e.target.value.replace(/\D/g, "");
        if (value.length > 11) value = value.slice(0, 11);

        if (value.length > 6) {
            e.target.value = `(${value.slice(0, 2)}) ${value.slice(2, 7)}-${value.slice(7)}`;
        } else if (value.length > 2) {
            e.target.value = `(${value.slice(0, 2)}) ${value.slice(2)}`;
        } else if (value.length > 0) {
            e.target.value = `(${value}`;
        }
    });

    
    form.addEventListener("submit", function (event) {
        event.preventDefault();

        msgErro.textContent = "";
        msgSucesso.textContent = "";

        const nome = document.getElementById("nome").value.trim();
        const email = document.getElementById("email").value.trim();
        const telefone = telefoneInput.value.trim();
        const idade = document.getElementById("idade").value;
        const modalidade = document.getElementById("modalidade").value;

        
        if (nome.length < 3) {
            msgErro.textContent = "⚠ Por favor, digite seu nome completo.";
            return;
        }

        if (telefone.length > 0 && telefone.length < 15) {
            msgErro.textContent = "⚠ Insira um telefone válido: (00) 99999-9999";
            return;
        }

       
        const dadosSkatista = {
            nome: nome,
            email: email,
            telefone: telefone,
            idade: idade,
            modalidade: modalidade,
            dataCadastro: new Date().toLocaleDateString('pt-BR')
        };

        
        const cadastrosExistentes = JSON.parse(localStorage.getItem("skatistasCadastrados")) || [];
        
        
        cadastrosExistentes.push(dadosSkatista);

     
        localStorage.setItem("skatistasCadastrados", JSON.stringify(cadastrosExistentes));

    
        msgSucesso.innerHTML = `🔥 <strong>Valeu, ${nome}!</strong> Cadastro salvo no navegador!<br>Modalidade: <strong>${modalidade.toUpperCase()}</strong>`;
        
        form.reset();
    });
});