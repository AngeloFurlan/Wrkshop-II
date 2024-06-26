# MOVEDU- Workshop 2

try:
  git.checkout('Wokshop')
except git.exc.GitError as e:
  print(f"Erro ao fazer checkout da tag 'Wokshop': {e}")
  # Cria um arquivo chamado "error_log.txt" com a mensagem de erro
  with open("error_log.txt", "w") as f:
    f.write(f"Erro: {e}")


Esse arquivo faz parte do repositório utilizado no workshop da faculdade Moveedu
