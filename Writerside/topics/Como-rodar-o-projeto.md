# Como rodar o projeto

Existem diversas maneiras de rodar o projeto, esta sessão mostrará todas as maneiras fáceis de executa-lo

## Com docker

> **Highlight important information**
>
> Antes de prosseguir com esse tópico verifique se você tem o [Docker](https://www.docker.com/) instalado e configurado na sua máquina.
>
{style="warning"}

### Antes de começar

Verifique se:
- A porta 5432 não está em uso
- A porta 8080 não está em uso
- A porta 3000 não está em uso
- A porta 11434 não está em uso

### Rodando

1. Execute o seguinte comando

   ```bash
    docker compose up -d
   ```

2. Step with a [link](http://localhost:3000/guma)

3. Step with a list.
   - Realize o login com sua conta Canvas
   - Siga o passo a passo para avaliar uma atividade

## Rodando manualmente

> **Highlight important information**
>
> Antes de prosseguir com esse tópico verifique se você tem o [Ollama](https://ollama.com/library), instalado e configurado na sua máquina.
>
{style="warning"}

Verifique se:
- A porta 8080 não está em uso
- A porta 3000 não está em uso
- A porta 11434 não está em uso

### Execute

1. Rode o ollama
```bash
ollama serve
```

2. Após isso faça o pull do seu modelo favorito com

```bash
ollama run seu_modelo
```

3. Após isso troque no ```aplication.yml``` para o modelo desejado no campo ```OLLAMA_MODEL``` e em seguida rode

```bash
mvn spring-boot:run
```

4. Step with a [link](http://localhost:3000/guma)

5. Step with a list.
   - Realize o login com sua conta Canvas
   - Siga o passo a passo para avaliar uma atividade