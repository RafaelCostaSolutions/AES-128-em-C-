# AES-128-em-C++

Implementação do algoritmo de criptografia AES-128 em C++. AES (Advanced Encryption Standard) é um dos algoritmos de criptografia mais utilizados e é conhecido por sua segurança e eficiência.

Explicação Detalhada
KeyExpansion:

Expande a chave original para gerar as chaves de cada rodada.
AddRoundKey:

Combina a chave de rodada com o estado usando a operação XOR.
SubBytes:

Substitui cada byte do estado pelo valor correspondente na S-box.
ShiftRows:

Desloca ciclicamente as linhas do estado para a esquerda.
MixColumns:

Mistura as colunas do estado usando operações de multiplicação no campo finito GF(2^8).
Cipher:

Implementa o ciclo principal do AES, que consiste em múltiplas rodadas de SubBytes, ShiftRows, MixColumns (exceto na última rodada) e AddRoundKey.
AES128_ECB_encrypt:

Realiza a criptografia de um bloco de 128 bits usando o modo de operação ECB (Electronic Codebook).
Função Principal:

Define uma chave e um texto claro de exemplo, chama a função de criptografia e imprime o texto cifrado.
