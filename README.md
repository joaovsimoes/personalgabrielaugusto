# Plataforma Gabriel Augusto

Portal oficial do Personal Trainer Gabriel Augusto, integrado ao Firebase.

## Serviços usados

- Firebase Authentication: acesso do personal e dos alunos.
- Cloud Firestore: alunos, anamneses, treinos, pagamentos, relatórios, notificações e imagens compactadas.
- GitHub Pages: publicação no domínio oficial.

O portal não depende do Firebase Storage. As fotos são compactadas antes do envio e os PDFs são gerados no navegador a partir dos dados privados do relatório.

## Publicação

Ative o provedor E-mail/Senha no Firebase Authentication, confirme que `www.plataformagabrielaugusto.com.br` está nos domínios autorizados e valide a conta administrativa.

```bash
firebase deploy --only firestore:rules
```

As regras de segurança do banco estão em `firestore.rules`. O projeto configurado em `.firebaserc` é `personal-trainer-gabriel-ea005`.
