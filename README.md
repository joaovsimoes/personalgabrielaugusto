# Plataforma Gabriel Augusto

Portal oficial do Personal Trainer Gabriel Augusto, integrado ao Firebase.

## Serviços usados

- Firebase Authentication: acesso do personal e dos alunos.
- Cloud Firestore: alunos, anamneses, treinos, pagamentos, relatórios e notificações.
- Firebase Storage: fotos e PDFs privados.
- Firebase Hosting: publicação no domínio oficial.

## Publicação

Antes do primeiro deploy, ative o provedor E-mail/Senha no Firebase Authentication, confirme que `www.plataformagabrielaugusto.com.br` está nos domínios autorizados e valide a conta administrativa.

```bash
firebase deploy --only firestore:rules,storage,hosting
```

As regras de segurança estão em `firestore.rules` e `storage.rules`. O projeto configurado em `.firebaserc` é `personal-trainer-gabriel-ea005`.
