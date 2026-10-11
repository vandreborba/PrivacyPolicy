# Rascunho — Política de Privacidade (EV Log)

> Copiar para: https://github.com/vandreborba/PrivacyPolicy/blob/main/ev_log.md
> (no Play Console, a URL pública é a versão "raw": https://raw.githubusercontent.com/vandreborba/PrivacyPolicy/main/ev_log.md)

---

## pt-BR (Português Brasileiro)

**POLÍTICA DE PRIVACIDADE — EV Log**
Última atualização: 5 de outubro de 2026
Desenvolvedor: VandreApps

---

### SOBRE O DESENVOLVEDOR

VandreApps é um desenvolvedor independente, atuando como pessoa física, sem vínculo com qualquer empresa. Todo o desenvolvimento, manutenção e suporte do aplicativo EV Log são feitos de forma autônoma e individual.

---

### 1. RESUMO

O EV Log registra recargas e viagens de um veículo elétrico e estima o consumo de energia em trajetos futuros. Por padrão, **seus dados ficam apenas no seu aparelho**.

Para calcular rotas e localizar pontos de recarga, o app envia à nuvem apenas as coordenadas necessárias, **sem nome, e-mail, telefone ou qualquer informação que identifique você**.

O app também coleta **dados de uso** (telas acessadas e ações realizadas) por meio do Firebase Analytics, para melhorar o aplicativo. Essa coleta vem ligada por padrão e **pode ser desativada a qualquer momento** em Opções.

O desenvolvedor **não vende dados**. O app exibe anúncios (Google AdMob, seção 7) e oferece compras e assinaturas (RevenueCat, seção 8).

---

### 2. DADOS NO APARELHO

Ficam **somente no seu dispositivo**:

- Veículos cadastrados (nome, capacidade da bateria, peso, saúde e calibração)
- Recargas e viagens registradas, incluindo o trajeto GPS gravado durante a viagem
- Simulações, histórico de rotas em cache e preferências do app

O desenvolvedor não tem acesso a esses dados. Eles permanecem no aparelho até você excluí-los no app ou desinstalá-lo.

---

### 3. LOCALIZAÇÃO (GPS)

A localização é usada para:

- Registrar o trajeto da viagem durante o percurso (o trajeto fica no aparelho)
- Preencher automaticamente a cidade dos trechos e o local de uma recarga

A localização **não é usada para anúncios nem para perfilamento** e não é vendida. Você pode negar ou revogar a permissão a qualquer momento nas configurações do Android; sem ela, o rastreamento e o preenchimento automático deixam de funcionar, mas o restante do app continua disponível.

---

### 4. DADOS ENVIADOS À NUVEM

Para o funcionamento das rotas, o app usa serviços do Google Firebase:

- Cria uma **conta anônima**, com um identificador aleatório, sem nome, e-mail ou senha. Ele serve apenas para aplicar limites de uso.
- Envia as **coordenadas de origem e destino** (e paradas) para calcular a rota e a estimativa de consumo.
- Envia a **região da rota** para localizar pontos de recarga próximos.

Esses dados são usados apenas para gerar o resultado e ficam em **cache temporário, sem vínculo com a sua identidade** (o cache serve para não repetir consultas e é compartilhado entre trechos iguais). O aplicativo também usa o Firebase App Check para proteger o backend contra uso indevido.

**Não são enviados:** seus registros de recargas e viagens, o trajeto GPS completo, o nome do veículo ou qualquer anotação pessoal.

---

### 5. DADOS DE USO (FIREBASE ANALYTICS)

O aplicativo coleta estatísticas de uso para entender como ele é utilizado e melhorá-lo:

- **Interações:** telas abertas e ações realizadas (por exemplo, calcular uma estimativa, registrar uma recarga ou uma viagem, usar o backup)
- **Informações técnicas:** modelo/versão do aparelho, versão do app, idioma e identificadores do aplicativo

Esses dados são **agregados e usados apenas para melhoria do app**. Não são usados para publicidade, não incluem o conteúdo que você registra (valores, endereços, anotações) e não são vendidos.

A coleta vem **ligada por padrão** e pode ser **desativada em Opções**; ao desativar, o app para de enviar esses dados. Os dados são processados pelo Google conforme a política do Firebase.

---

### 6. SERVIÇOS DE TERCEIROS

O app utiliza os seguintes serviços, que recebem apenas os dados técnicos necessários:

- **Google Firebase / Google Cloud** — autenticação anônima, funções, cache e analytics. [Privacidade](https://firebase.google.com/support/privacy)
- **OpenRouteService (HeiGIT)** — cálculo de rota e altimetria
- **OpenStreetMap / Nominatim** — mapas e conversão entre endereço e coordenadas. [Privacidade](https://osmfoundation.org/wiki/Privacy_Policy)
- **Open Charge Map** — pontos de recarga. [Privacidade](https://openchargemap.org/site/about/privacy)
- **Google Play Store** — distribuição do aplicativo

- **Google AdMob** — exibição de anúncios (seção 7)
- **RevenueCat** — gestão de compras e assinaturas (seção 8)

---

### 7. PUBLICIDADE (GOOGLE ADMOB)

O aplicativo exibe anúncios por meio do **Google AdMob**. Para exibir e medir anúncios, o AdMob pode usar o **identificador de publicidade** do aparelho, o IP aproximado e informações técnicas (modelo do aparelho, sistema e versão do app). Nenhum dado que você registra no app (viagens, recargas, trajetos) é enviado ao AdMob.

Você pode limitar anúncios personalizados nas configurações do Android ou em [adssettings.google.com](https://adssettings.google.com/). Desativar a personalização não remove os anúncios, apenas os torna menos relevantes.

---

### 8. COMPRAS E ASSINATURAS (REVENUECAT)

O app oferece compras e assinaturas gerenciadas pelo **RevenueCat**, que processa dados da compra (produto adquirido, histórico e status) para liberar os recursos e restaurar compras. **Os dados de pagamento são processados pelo Google Play** e não passam pelo desenvolvedor. [Privacidade](https://www.revenuecat.com/privacy)

---

### 9. FINALIDADES E BASE LEGAL

Os dados são tratados para: funcionamento do app, cálculo de rotas e estimativas, localização de recargas, **melhoria do aplicativo**, exibição de anúncios, gestão de compras e assinaturas, e segurança contra uso indevido.

Base legal conforme a LGPD (Lei nº 13.709/2018): consentimento e execução do serviço ao usar o app e conceder permissões; legítimo interesse para analytics e segurança, sempre com o mínimo necessário.

---

### 10. COMPARTILHAMENTO E TRANSFERÊNCIA INTERNACIONAL

O desenvolvedor **não vende nem aluga dados**. Os dados técnicos descritos são processados pelos provedores citados (Google, HeiGIT, OpenStreetMap, Open Charge Map, AdMob e RevenueCat), conforme as políticas deles. Esses provedores podem processar dados em servidores **fora do Brasil**.

---

### 11. SEGURANÇA

As chamadas à nuvem usam **HTTPS/TLS** e o backend é protegido por autenticação e App Check. Os dados locais dependem da segurança física do aparelho.

Este é um projeto independente, mantido por uma pessoa, sem equipe de segurança dedicada. Foram adotadas medidas razoáveis, mas **não é possível garantir proteção absoluta** contra falhas ou acessos não autorizados decorrentes de serviços de terceiros ou dispositivos comprometidos.

---

### 12. RETENÇÃO

- **Dados locais:** até você excluí-los no app ou desinstalar.
- **Dados na nuvem (rotas, recargas, contadores):** mantidos apenas pelo tempo necessário ao funcionamento e removidos automaticamente.
- **Dados de uso (Analytics):** retidos conforme a política do Google Firebase.
- **Dados de anúncios e de compras:** retidos conforme as políticas do Google/AdMob e do RevenueCat.

---

### 13. DIREITOS DO USUÁRIO

Você pode, a qualquer momento:

- **Excluir** registros no app e **apagar tudo** desinstalando-o
- **Exportar** seus dados em um backup
- **Desativar** o envio de dados de uso em Opções
- **Revogar** as permissões de localização e notificações no Android

---

### 14. CRIANÇAS

O aplicativo não é direcionado a crianças e não coleta intencionalmente dados de menores. Ele não solicita nome, e-mail ou qualquer dado pessoal.

---

### 15. ALTERAÇÕES

Esta política pode ser atualizada. A data no topo indica a versão vigente. O uso continuado após uma atualização representa concordância com a nova versão.

---

### 16. CONTATO

Dúvidas sobre esta política: **vandreapps@gmail.com**

---

### 17. DECLARAÇÃO DO DESENVOLVEDOR

- Os dados de recargas, viagens e configurações permanecem **no aparelho do usuário**.
- O acesso à nuvem usa **login anônimo**, sem nome, e-mail ou telefone; as coordenadas servem só para calcular rota/consumo e localizar recargas.
- O **trajeto GPS completo** não é enviado à nuvem.
- O app coleta **dados de uso** (telas e ações) para melhoria, **desativáveis em Opções**, sem conteúdo pessoal e sem venda de dados.
- O app **não solicita** câmera, microfone ou contatos.
- O app exibe **anúncios** (Google AdMob) e oferece **compras e assinaturas** (RevenueCat), conforme as seções 7 e 8.

---

Ao utilizar o aplicativo EV Log, você concorda com esta Política de Privacidade.

---
---

## en-US (English)

**PRIVACY POLICY — EV Log**
Last updated: October 5, 2026
Developer: VandreApps

---

### ABOUT THE DEVELOPER

VandreApps is an independent developer, operating as an individual, without affiliation to any company. All development, maintenance, and support of the EV Log application are performed autonomously and individually.

---

### 1. SUMMARY

EV Log logs electric-vehicle charging sessions and trips and estimates energy consumption on future routes. By default, **your data stays only on your device**.

To calculate routes and find charging points, the app sends to the cloud only the necessary coordinates, **with no name, email, phone number or anything that identifies you**.

The app also collects **usage data** (screens visited and actions performed) through Firebase Analytics to improve the application. This collection is on by default and **can be disabled at any time** in Options.

The developer **does not sell data**. The app shows ads (Google AdMob, Section 7) and offers purchases and subscriptions (RevenueCat, Section 8).

---

### 2. DATA ON THE DEVICE

Kept **only on your device**:

- Registered vehicles (name, battery capacity, weight, health and calibration)
- Charging and trip records, including the GPS track recorded during a trip
- Simulations, cached routes and app preferences

The developer has no access to this data. It stays on the device until you delete it in the app or uninstall the app.

---

### 3. LOCATION (GPS)

Location is used to:

- Record the trip path while driving (the track stays on the device)
- Automatically fill in each leg's city and the place of a charging session

Location is **not used for ads or profiling** and is not sold. You can deny or revoke the permission at any time in Android settings; without it, tracking and auto-fill stop working, but the rest of the app remains available.

---

### 4. DATA SENT TO THE CLOUD

To provide routes, the app uses Google Firebase services:

- It creates an **anonymous account** with a random identifier, with no name, email or password. It is used only to enforce usage limits.
- It sends the **origin and destination coordinates** (and stops) to calculate the route and consumption estimate.
- It sends the **route area** to find nearby charging points.

This data is used only to produce the result and is kept in **temporary cache, with no link to your identity** (the cache avoids repeating queries and is shared between identical legs). The app also uses Firebase App Check to protect the backend against misuse.

**Not sent:** your charging and trip records, the full GPS track, vehicle names or any personal notes.

---

### 5. USAGE DATA (FIREBASE ANALYTICS)

The app collects usage statistics to understand how it is used and to improve it:

- **Interactions:** screens opened and actions performed (for example, calculating an estimate, logging a charge or a trip, using backup)
- **Technical information:** device model/version, app version, language and app identifiers

This data is **aggregated and used only to improve the app**. It is not used for advertising, does not include the content you record (amounts, addresses, notes) and is not sold.

Collection is **on by default** and can be **disabled in Options**; when you disable it, the app stops sending this data. The data is processed by Google under the Firebase privacy policy.

---

### 6. THIRD-PARTY SERVICES

The app uses the following services, which receive only the technical data required:

- **Google Firebase / Google Cloud** — anonymous authentication, functions, cache and analytics. [Privacy](https://firebase.google.com/support/privacy)
- **OpenRouteService (HeiGIT)** — route and elevation calculation
- **OpenStreetMap / Nominatim** — maps and address↔coordinates conversion. [Privacy](https://osmfoundation.org/wiki/Privacy_Policy)
- **Open Charge Map** — charging points. [Privacy](https://openchargemap.org/site/about/privacy)
- **Google Play Store** — app distribution

- **Google AdMob** — ad display (Section 7)
- **RevenueCat** — purchase and subscription management (Section 8)

---

### 7. ADVERTISING (GOOGLE ADMOB)

The application displays ads through **Google AdMob**. To serve and measure ads, AdMob may use the device **advertising identifier**, approximate IP and technical information (device model, system and app version). No content you record in the app (trips, charges, tracks) is sent to AdMob.

You can limit personalized ads in Android settings or at [adssettings.google.com](https://adssettings.google.com/). Turning off personalization does not remove ads, it only makes them less relevant.

---

### 8. PURCHASES AND SUBSCRIPTIONS (REVENUECAT)

The app offers purchases and subscriptions managed by **RevenueCat**, which processes purchase data (product, history and status) to unlock features and restore purchases. **Payment data is processed by Google Play** and does not pass through the developer. [Privacy](https://www.revenuecat.com/privacy)

---

### 9. PURPOSES AND LEGAL BASIS

Data is processed to: run the app, calculate routes and estimates, find charging points, **improve the application**, display ads, manage purchases and subscriptions, and protect against misuse.

Legal basis under the Brazilian LGPD (Law No. 13,709/2018): consent and performance of the service when you use the app and grant permissions; legitimate interest for analytics and security, always with the minimum necessary.

---

### 10. SHARING AND INTERNATIONAL TRANSFER

The developer **does not sell or rent data**. The technical data described is processed by the providers listed (Google, HeiGIT, OpenStreetMap, Open Charge Map, AdMob and RevenueCat), under their policies. These providers may process data on servers **outside Brazil**.

---

### 11. SECURITY

Cloud calls use **HTTPS/TLS** and the backend is protected by authentication and App Check. Local data depends on the physical security of your device.

This is an independently developed project, maintained by one person, without a dedicated security team. Reasonable measures have been taken, but **absolute protection cannot be guaranteed** against failures or unauthorized access resulting from third-party services or compromised devices.

---

### 12. RETENTION

- **Local data:** until you delete it in the app or uninstall.
- **Cloud data (routes, charges, counters):** kept only as long as needed to work and removed automatically.
- **Usage data (Analytics):** retained under Google Firebase's policy.
- **Ads and purchase data:** retained under the Google/AdMob and RevenueCat policies.

---

### 13. USER RIGHTS

You may, at any time:

- **Delete** records in the app and **erase everything** by uninstalling it
- **Export** your data to a backup
- **Disable** usage-data collection in Options
- **Revoke** location and notification permissions in Android

---

### 14. CHILDREN

The app is not directed to children and does not intentionally collect data from minors. It does not request a name, email or any personal data.

---

### 15. CHANGES

This policy may be updated. The date at the top indicates the current version. Continued use after an update means agreement with the new version.

---

### 16. CONTACT

Questions about this policy: **vandreapps@gmail.com**

---

### 17. DEVELOPER DECLARATION

- Charging, trip and settings data remains **on the user's device**.
- Cloud access uses **anonymous sign-in**, with no name, email or phone; coordinates are used only to calculate route/consumption and find charging points.
- The **full GPS track** is not sent to the cloud.
- The app collects **usage data** (screens and actions) for improvement, **disableable in Options**, with no personal content and no data selling.
- The app **does not request** camera, microphone or contacts.
- The app shows **ads** (Google AdMob) and offers **purchases and subscriptions** (RevenueCat), as described in Sections 7 and 8.

---

By using the EV Log application, you agree to this Privacy Policy.
