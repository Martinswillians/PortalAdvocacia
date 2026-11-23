# Portal AAB – guia de implantação

## 1. Firebase (projeto portaladvocacia)
1. **Firestore → Regras**: cole o conteúdo de `firestore.rules` e clique em **Publicar**.
2. **Authentication → Users → Adicionar usuário**: e-mail `willbrasilia@gmail.com` + a senha padrão combinada.
   (A senha NÃO está no código, que é público no GitHub. Faça isso logo, antes de publicar o site.)
3. **Authentication → Configurações → Domínios autorizados**: adicione `martinswillians.github.io`.
4. Depois do primeiro login, abra **Administração → Configurações → Trocar senha** e defina uma senha forte.

## 2. GitHub Pages (repositório Martinswillians/PortalAdvocacia, branch main, raiz)
Envie para a raiz: `index.html`, `sw.js`, `manifest.webmanifest` e a pasta `icons/`.
Endereço: https://martinswillians.github.io/PortalAdvocacia/

## 3. Como funciona
- **Administrador** (willbrasilia@gmail.com) vê o menu *Administração*: resumo, associados (aprovar, suspender, recusar, excluir, ver quem está online e último acesso), comunicados (aviso, alerta, publicação, atualização; fixar, expirar, pop-up, público ou só associados), acessos e configurações (aprovação automática, textos).
- **Advogado** cria conta em *Associar-se*; fica "pendente" até a AAB aprovar (ou entra direto se a aprovação automática estiver ligada). Depois cria o site em *Meu site*, em `#/a/<endereço>`.
- Comunicados marcados como **pop-up** aparecem ao logar/criar conta; os públicos aparecem na página inicial.
- Suspender um associado tira o site do ar.
- Os índices do Firestore não são necessários.
