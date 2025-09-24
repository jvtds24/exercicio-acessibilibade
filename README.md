## ♿ Acessibilidade com HTML Semântico e ARIA

Este projeto foi desenvolvido com um forte foco em acessibilidade, garantindo que a aplicação seja utilizável por todos, incluindo pessoas que dependem de tecnologias assistivas como leitores de tela.

Nossa abordagem se baseia em duas práticas fundamentais:

1.  **HTML Semântico (A Base de Tudo):** Priorizamos o uso de tags HTML nativas e semanticamente corretas. Elementos como `<button>`, `<h1>`, `<a>`, e `<p>` já possuem acessibilidade embutida, comunicando sua função diretamente ao navegador e às tecnologias assistivas.

2.  **ARIA (Quando o Semântico Não é Suficiente):** Onde componentes dinâmicos e personalizados foram criados, utilizamos atributos ARIA (Accessible Rich Internet Applications) para adicionar contexto e clareza.

### Aplicações de ARIA no Projeto

-   **Navegação Principal:** Usamos `aria-label="Menu Principal"` para dar um nome acessível à seção de navegação, facilitando sua identificação.
-   **Rodapé:** A tag `<footer>` já possui a `role="contentinfo"` implícita. Adicionamos o atributo explicitamente como reforço, embora o uso da tag semântica por si só já seja a prática recomendada.

### Exemplo Prático: Componente `Switch` Acessível

Para demonstrar um cenário onde ARIA é essencial, criamos um componente de **Switch** (interruptor), que não existe nativamente em HTML. Para torná-lo acessível, aplicamos os seguintes atributos:

-   `role="switch"`: Informa à tecnologia assistiva que o elemento se comporta como um interruptor.
-   `aria-checked`: Comunica o estado atual do componente ("true" para ligado, "false" para desligado).

Este exemplo ilustra como construir componentes de interface complexos e garantir que eles sejam totalmente acessíveis.
