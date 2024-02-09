-- Criando uma variável para armazenar a key
local key = "GHOST"

-- Criando uma variável para armazenar a gui
local gui = script.Parent

-- Criando uma variável para armazenar o campo de usuário
local userEdit = gui.UserEdit

-- Criando uma variável para armazenar o campo de senha
local passEdit = gui.PassEdit

-- Criando uma variável para armazenar o botão de login
local loginButton = gui.LoginButton

-- Criando uma função para verificar se o usuário e a senha estão corretos
local function checkLogin()
  -- Pegando o texto digitado pelo usuário
  local user = userEdit.Text
  local pass = passEdit.Text

  -- Verificando se o usuário e a senha são iguais à key
  if user == key and pass == key then
    -- Mostrando uma mensagem de sucesso
    print("Login bem sucedido!")
    -- Fechando a gui
    gui.Visible = false
  else
    -- Mostrando uma mensagem de erro
    print("Usuário ou senha incorretos!")
  end
end

-- Conectando a função ao evento de clique do botão
loginButton.MouseButton1Click:Connect(checkLogin)
: ...

<!---
Dhiogo032/Dhiogo032 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
