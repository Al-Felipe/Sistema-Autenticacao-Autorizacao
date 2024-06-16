# Sistema de Autenticação e Autorização

## Objetivo
Implementar um sistema de autenticação segura utilizando JSON Web Tokens (JWT), 
permitindo acesso a endpoints especificos de acordo com o nível de permissão do usuário podendo este ser
(ADMIN, MODERADOR E COMUM).

## Diagrama de Classes

<img width="2583" alt="diagrama" src="https://github.com/Al-Felipe/Sistema-Autenticacao-Autorizacao/assets/105646899/6d754553-e9d2-4501-b3cd-eaf6da7c98e3">

## APIs disponíveis para utilização

**POST** /login: Endpoint de autenticação para obter token JWT.

Endpoint: https://exemplo.com/login

![post login](https://github.com/Al-Felipe/Sistema-Autenticacao-Autorizacao/assets/105646899/e813c37b-49cf-49d0-ba1b-864ba5c7cdd7)

**GET** /username/{token}: Retorna o nome do usuário a partir do token JWT.

Endpoint: https://exemplo.com/username/{token}

![get username](https://github.com/Al-Felipe/Sistema-Autenticacao-Autorizacao/assets/105646899/53d039ff-963b-4b34-b827-9a399675eb3b)

**GET** /user: Retorna informações sobre o usuário autenticado.

Endpoint: https://exemplo.com/user

![get user](https://github.com/Al-Felipe/Sistema-Autenticacao-Autorizacao/assets/105646899/b2bc699c-bf6b-456f-9c0a-77a73db14c07)

**GET** /admin: Disponível apenas para usuários com a função de ADMIN.

Endpoint: https://exemplo.com/admin

![get admin](https://github.com/Al-Felipe/Sistema-Autenticacao-Autorizacao/assets/105646899/aedc9e40-654d-4f61-a2da-2f174d0bddd6)

**GET** /moderador: Disponível apenas para usuários com a função de MODERADOR.

Endpoint: https://exemplo.com/moderador

![get moderador](https://github.com/Al-Felipe/Sistema-Autenticacao-Autorizacao/assets/105646899/95f4ed52-5623-4ea5-8dd8-815225fc5c97)

**GET** /comum: Disponível para usuários comuns.

Endpoint: https://exemplo.com/comum

![get comum](https://github.com/Al-Felipe/Sistema-Autenticacao-Autorizacao/assets/105646899/3194c16d-dca5-4bcc-a7d8-9e4713fc741f)

## Usuário não autenticado

Aplicação não permite que usuários sem autorização acessem determinados endpoints.

![nao autorizado](https://github.com/Al-Felipe/Sistema-Autenticacao-Autorizacao/assets/105646899/5e6ac7c5-4032-4432-b0cd-77fe4c22b67a)



