# LINUXtips-PICK
Desafio de Projeto Prático - PICK 2024_01

Primeiro projeto prático do PICK - Programa Intensivo em Containers e Kubernetes 2024 ministrado pela @LINUXtips.

O objetivo do projeto é criar uma aplicação de gestão de senhas baseada no projeto giropops-senhas, utilizando Docker, Kubernetes, Helm, Kyverno, Cosign, Prometheus, apko e Melange para garantir a segurança, automação, e monitoramento contínuo da aplicação.

#### ⭐ Requisitos do Projeto:

1. **Containerização com Docker:**
   - Containerizar a aplicação de gestão de senhas.
   - Criar um `Dockerfile` eficiente e seguro.
   - Publicar a imagem Docker em um repositório privado.

2. **Orquestração com Kubernetes:**
   - Implementar a aplicação no Kubernetes.
   - Criar os manifests necessários (`Deployment`, `Service`, `ConfigMap`, `Secret`, etc.).
   - Utilizar `Ingress` para expor a aplicação externamente.

3. **Automação de Deploy com Helm:**
   - Criar um Chart Helm para a aplicação.
   - Configurar valores dinâmicos para diferentes ambientes (dev, staging, prod).
   - Gerar pacotes Helm e armazenar em um repositório Helm privado.

4. **Políticas de Segurança com Kyverno:**
   - Criar políticas Kyverno para garantir práticas de segurança, como:
     - Verificação de imagens assinadas.
     - Proibição de execução como root.
     - Verificação de variáveis de ambiente sensíveis.
   - Implementar políticas de conformidade (compliance).

5. **Assinatura de Imagens com Cosign:**
   - Assinar as imagens Docker utilizando Cosign.
   - Configurar a verificação automática das assinaturas no Kubernetes utilizando as políticas Kyverno.

6. **Monitoramento com Prometheus:**
   - Implementar métricas customizadas na aplicação.
   - Configurar Prometheus para coletar e visualizar essas métricas.
   - Criar alertas baseados em métricas específicas da aplicação.

7. **Distribuição de Pacotes com APKO e Melange:**
   - Utilizar Melange para criar pacotes da aplicação.
   - Configurar um pipeline CI/CD para construir e distribuir esses pacotes.
   - Garantir que os pacotes estejam disponíveis para diferentes ambientes (dev, staging, prod).
