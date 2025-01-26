# Variational-Autoencoders-VAE
Este repositório contém uma implementação do Variational Autoencoder (VAE), um modelo generativo que aprende representações latentes probabilísticas. Ao contrário dos autoencoders tradicionais, o VAE modela a distribuição do espaço latente, permitindo gerar novas amostras e realizar reconstruções de dados com alta qualidade.

Este repositório inclui:

- Arquitetura do Autoencoder Variacional: O VAE é composto por um encoder, responsável por mapear as imagens para o espaço latente, e um decoder, que reconstrói as imagens a partir desse espaço latente. O modelo é treinado para otimizar a reconstrução das imagens e minimizar a discrepância entre a distribuição latente aprendida e uma distribuição normal padrão.

- Amostragem Latente e Perda KL: A principal inovação do VAE é a introdução de uma regularização no treinamento por meio da perda Kullback-Leibler (KL). Essa perda assegura que o espaço latente do modelo siga uma distribuição normal padrão, facilitando a geração de novas amostras. A camada de amostragem realiza a amostragem do vetor latente a partir dessa distribuição.

- Função de Perda: O modelo é treinado para minimizar uma combinação de duas perdas: a perda de reconstrução, que mede a qualidade da reconstrução das imagens, e a perda KL, que garante que a distribuição latente seja próxima da distribuição normal desejada.

- Treinamento e Avaliação: O VAE foi treinado por 200 épocas, com ajustes no processo de otimização para garantir que o modelo aprenda uma representação latente que capture as características essenciais dos dados, ao mesmo tempo em que seja capaz de gerar novas amostras com alta qualidade.

Objetivo:

O objetivo deste projeto foi avaliar a capacidade do Variational Autoencoder em gerar novas amostras e reconstruir imagens com alta qualidade, a partir de uma representação latente probabilística. Ao modelar a distribuição dos dados no espaço latente, o VAE permite não apenas realizar boas reconstruções, mas também gerar novas imagens que seguem a mesma distribuição dos dados originais. Esse poder gerativo é útil em diversas aplicações, como a geração de novas imagens ou remoção de ruído em imagens ruidosas, ao reconstruir imagens de forma robusta a partir do espaço latente aprendido.
