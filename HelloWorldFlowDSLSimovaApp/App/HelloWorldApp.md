// Modulo App: determina as configurações globais do aplicativo.

// Linha 4: parâmetro [appCode] é usado pelo Web Service para determinar alguns comportamentos do aplicativo.
App appCode=HelloWorld
  // Linha 6: parâmetro [name] que determina qual será o nome do aplicativo exibido para o usuário ao configurar o fluxo no core.
  name HelloWorldApp
  // Linha 8: determina o comportamento da comunicação com o Web Service
  server
  // Linha 10: parâmetro [url] que determina a URL para a comunicação com o Web Service
  jsonServiceApi url=https://xmova-center-dev.simova.ws/fakewebservice
  // Linha 12: determina o modo de controle do versionamento dos dados cadastrais recebidos pelo aplicativo
  versionControl Crc

// Linha 15: determina o nome da tela e a segunda parte [main] indica que esta é a tela principal do aplicativo
Main main
  // Linha 17: determina as ações que serão disponibilizadas para o usuário na tela principal
  actions
    // Linha 19: declaração da única ação da tela principal que é a ação [Iniciar] sendo do tipo [OK]
    Iniciar Ok
      // Linha 21: declaração do bloco de instrução que será executado quando o usuário pressionar a ação [Iniciar]
      crud Boletim
