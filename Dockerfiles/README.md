
# Curso Full Cyple

## Módulo Docker

### Projeto Go: Uma imagem go com no máximo 2MB.
Para fazer o dockerfile foi utilizado multistage building para diminuir o tamanho da imagem final.
No primeiro passo é gerado o binario. No segundo passo esse binario é copiado para um container scratch, para finalmente ser executado.
