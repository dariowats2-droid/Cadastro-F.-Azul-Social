Cadastro Social+ - Protótipo Flutter
===================================

O pacote contém os arquivos principais do protótipo do aplicativo **Cadastro Social+**.

O que está incluído:
- lib/main.dart  -> Código fonte do protótipo (single-file)
- pubspec.yaml   -> Dependências necessárias

Como gerar e instalar o APK (no seu computador com Flutter + Android SDK configurados):

1. Instale Flutter: https://flutter.dev/docs/get-started/install
2. Crie um novo projeto Flutter (opcional) ou use este diretório:
   - Se quiser criar um projeto novo:
     flutter create cadastro_social_plus_app
     cd cadastro_social_plus_app
     rm -rf lib
     cp -r /caminho/para/extraido/lib ./lib
     cp /caminho/para/extraido/pubspec.yaml .

   - Ou substitua os arquivos do seu projeto pelos deste pacote.

3. No diretório do projeto, rode:
   flutter pub get

4. Conecte um dispositivo Android ou configure um emulador.

5. Gere o APK:
   flutter build apk --release

6. O APK será gerado em:
   build/app/outputs/flutter-apk/app-release.apk

7. Transfira e instale no seu aparelho Android:
   adb install -r build/app/outputs/flutter-apk/app-release.apk

Se não tiver ambiente Flutter local, você pode:
- Pedir a alguém com Flutter configurado para rodar os passos acima.
- Ou posso ajudar a configurar um fluxo de CI (GitHub Actions) que gera o APK automaticamente a partir de um repositório (posso criar os arquivos de workflow também).

Observações:
- Este é um protótipo funcional; para produção é recomendável modularizar o código, adicionar tratamento de permissões, testes e assinar o APK para publicação.
- Se quiser, eu posso:
  - Preparar o repositório Git com CI para gerar APKs automaticamente.
  - Modularizar o projeto (separar em múltiplos arquivos).
  - Gerar assets (logo) e aprimorar a UI.