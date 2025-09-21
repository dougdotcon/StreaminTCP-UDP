# Introdução ao Protocolo UDP com Redundância de Dados

---

## Conceito Geral

Essa abordagem utiliza um protocolo customizado sobre UDP que, ao invés de depender de confirmações (ACKs) e retransmissões típicas do TCP, emprega uma técnica de **diluição** dos dados. A partir de N bytes, gera-se k × N bytes redundantes, permitindo reconstrução da mensagem mesmo com perdas, semelhante a códigos FEC.

---

## Funcionalidades

- **Adaptação dinâmica da redundância:** ajusta o fator de diluição conforme as condições do canal.
- **Redução da latência:** elimina overhead de ACKs e retransmissões.
- **Robustez e tolerância a erros:** garante reconstrução mesmo com perdas significativas.
- **Eficiência na utilização da banda:** evita desperdício com retransmissões.

---

## Aplicações Gerais

- **Transmissão de vídeo em tempo real:** vigilância, drones, transmissões ao vivo.
- **Redes IoT em ambientes adversos:** rural, industrial, dispositivos limitados.
- **Transmissões multicast:** distribuição eficiente para múltiplos receptores.
- **Sistemas aeroespaciais e satélites:** comunicações de longa distância sem retransmissão.

---