# MOVEDU- Workshop 2
import smtplib

# Configurações do email (substitua com suas informações)
smtp_server = "smtp.example.com"
smtp_port = 587
sender_email = "seuemail@example.com"
receiver_email = "equipe@example.com"
password = "suasenha"

# Conteúdo do email
subject = "Erro no Checkout da Tag 'Wokshop'"
message = f"Ocorreu um erro ao fazer checkout da tag 'Wokshop' no repositório Git.\n\nDetalhes do erro:\n{e}"

# Criar a conexão SMTP
with smtplib.SMTP(smtp_server, smtp_port) as server:
  server.starttls()
  server.login(sender_email, password)

  # Enviar o email
  server.sendmail(sender_email, receiver_email, message.encode('utf-8'))

Esse arquivo faz parte do repositório utilizado no workshop da faculdade Moveedu
