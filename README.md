# Forza AMD Universal Fix (APUs & Dedicadas)
FH201 &amp; FH205 Fix

Este é um fix experimental focado em contornar os erros FH201, FH205 e os congelamentos em tela preta causados pelo motor gráfico ForzaTech ao lidar com limitações de silício e subalocação de memória (VRAM).

Esta versão adiciona hooks avançados diretamente na vtable do DirectX 12 para resolver o problema da VRAM, além de forçar a exposição de suporte a Shader Model 6.6 e Enhanced Barriers para compatibilidade com o motor gráfico.

A DLL proxy atua como camada de compatibilidade para requisitos modernos do motor gráfico, mas a tradução física das instruções modernas ainda depende obrigatoriamente do driver modificado instalado no sistema.

# Passo a Passo

1. Baixe os arquivos da última versão deste repositório.
2. Acesse a pasta bin
3. Instale o Driver [AMD Software Adrenalin Edition - Agility SDK / Work Graphs](https://www.amd.com/en/resources/support-articles/release-notes/RN-RAD-MS-AGILITY-SDK-2023-6-711.html)
4. Copie os arquivos d3d12.dll e dxgi.dll
5. Cole os dois arquivos diretamente no diretório principal do jogo (onde está localizado o executável .exe)
6. Inicialize o jogo normalmente.

### Após Instalar o Driver para uma melhor experiência e recomendável reiniciar o Sistema.
