# SUBIR SO PARA CASO EU NAO TENHA ACESSO AO MEU COMPUTADOR


#ALTERAÇÕES FEITAS
- Mudei a class Pessoa, alterei id para string e removi static no set,get.
- Mudei a forma que os tx eram chamados, pode ser chamado pela variavel umapessoa.
- Dentro da pasta Debug, esta o BDCadPessoa, para conectar ao banco de dados, quie esta senod chamado na class DAL.

# PENDENCIAS QUE DEIXEI.
- Conexão com o bando de dados esta dando problema.
- O erro ocorreu apos eu adicinar essas linhas no Form1.cs.
- FormLoad esta abaixo do buttao1
- FormCloding esta no final do código


private void FormCadastro_Load(object sender, EventArgs e)
{
    PessoaBLL.conecta();
    if (Erro.getErro())
        MessageBox.Show(Erro.getMsg());
}

private void CadFormCadastro_FormClosing(object sender, FormClosingEventArgs e)
 {
     PessoaBLL.desconectar();
 }


-Quando adicionada uma pessoa incrementar um ID para cada uma(+=1).
-Dar funcionalidade para os botões basicos, eu fiz todas as verificações ja, mas eles ainda n salvam/excluem nada.
