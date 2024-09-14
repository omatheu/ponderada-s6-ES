# Proposta de Melhoria de Segurança em Sistema Conversacional

## 1. Introdução

**Descrição do problema**:  
A segurança em sistemas conversacionais é um aspecto crítico, especialmente em aplicações que lidam com dados sensíveis, como informações pessoais, financeiras ou (no caso do projeto deste módulo) leis que impactam o mercado financeiro. A falta de medidas de segurança robustas pode levar a vulnerabilidades, como ataques de intercepção de dados, ataques de injeção, violações de privacidade e acesso não autorizado a informações. Estas falhas podem comprometer tanto a integridade do sistema quanto a confiança dos usuários.

**Justificativas**:  
Com o aumento no uso de chatbots e assistentes virtuais, é essencial garantir que a comunicação entre o usuário e o sistema seja protegida. Além disso, sistemas que armazenam ou processam informações sensíveis devem aderir às melhores práticas de segurança, como criptografia de dados, autenticação robusta e controle de acesso. Bem como, no caso de uso de LLM's, é preciso previnir ataques com prompts maliciosos.

## 2. Solução Proposta

**Diagrama de Arquitetura**:  
(Insira aqui o diagrama de arquitetura do sistema, destacando os módulos relacionados à segurança, como autenticação, criptografia e firewall).

**Descrição Textual dos Módulos**:

- **Autenticação e Autorização**: Este módulo será responsável por garantir que apenas usuários autorizados possam acessar o sistema. Ele implementará autenticação multifator (MFA) e uso de tokens JWT para sessões seguras.
  
- **Criptografia de Dados**: Todos os dados trocados entre o cliente e o servidor serão criptografados utilizando TLS para proteger contra ataques de interceptação. Além disso, dados sensíveis armazenados serão criptografados em repouso.
  
- **Monitoramento e Auditoria**: O sistema incluirá um módulo de auditoria que registra todas as ações dos usuários, permitindo o rastreamento de atividades suspeitas. Logs de segurança serão analisados para detecção de anomalias.
  
- **Firewall e Filtragem de Tráfego**: Este módulo protegerá o sistema contra ataques de negação de serviço (DDoS) e limitará o acesso apenas a endereços IP autorizados.

## 3. Conclusão

**Considerações pessoais**:  
A proposta de melhoria para a segurança no sistema conversacional envolve um esforço considerável, especialmente na integração de múltiplas camadas de segurança, como criptografia, autenticação multifator e monitoramento contínuo. No entanto, os benefícios superam os custos, pois garantem maior confiabilidade e proteção de dados sensíveis dos usuários.

**Esforço para implementação**:  
A implementação dessas melhorias exigirá a integração de bibliotecas e serviços externos de segurança, como provedores de autenticação e APIs de criptografia. Também será necessário monitorar o sistema constantemente para identificar possíveis falhas ou vulnerabilidades emergentes.

## 4. Referências Bibliográficas

- Norma ISO 27001: o que é, funções e como implementar - Serasa Experian. Disponível em: <https://www.serasaexperian.com.br/blog-pme/iso-27001/>.
- Practical Attacks on LLMs: Full Guide | Iterasec. Disponível em: <https://iterasec.com/blog/practical-attacks-on-llms/#:~:text=Adversarial%20attacks%2C%20such%20as%20prompt>. Acesso em: 14 set. 2024.
- LLM Attacks. Disponível em: <https://github.com/llm-attacks/llm-attacks>.
