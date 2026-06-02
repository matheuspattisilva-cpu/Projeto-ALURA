# Projeto-ALURA

// Função separada para calcular o total, deixando o código limpo
function calcularTotal(quantidade, preco) {
    return quantidade * preco;
}

// Função principal que inicia o sistema
function iniciarSistema() {
    // Busca os valores dos inputs na tela
    const quantidade = document.getElementById("qtd").value;
    const preco = document.getElementById("preco").value;

    // Chama a função que criamos para fazer a conta
    const total = calcularTotal(quantidade, preco);

    // Verifica se o valor é alto
    if (total > 1000) {
        alert("Valor alto!");
    }

    // Mostra o resultado na tela
    document.getElementById("resultado").innerText = total;
}
