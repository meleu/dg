---
{"dg-publish":true,"permalink":"/notes/aprenda-rust-bruno-rocha/"}
---

# Aprenda Rust - Bruno Rocha

Playlist: <https://youtube.com/playlist?list=PLjSf4DcGBdiGCNOrCoFgtj0KrUq1MRUME>


## Introdução à linguagem Rust

<https://youtu.be/zWXloY0sslE>

`hello.rs`:
```rust
fn main() {
  println!("Hello World!");
}
```

Compilar:
```shell
# isso vai gerar um binário chamado 'hello'
rustc hello.rs
```

Compilar desta 👆 forma só é utilizado para coisinhas rápidas.

Normalmente usamos o `cargo` para gerenciar pacotes e outras coisas relacionadas ao projeto.

Iniciando um novo projeto:
```shell
cargo new my_project
# isso vai criar um dir com essa estrutura:
# my_project
# ├── Cargo.toml
# └── src
#     └── main.rs
```

**NOTA**: sempre que um diretório tiver um `Cargo.toml` válido, podemos dizer que é um workspace do Rust.

Fazer build do projeto:
```shell
# faz o build do projeto:
cargo build
# isso vai criar o dir 'target/'
# o binário vai para 'target/debug/my_project'

# executa o projeto
cargo run

# formatar o código
cargo fmt
```

## Variáveis e Constantes

<https://youtu.be/GYhTFLdHNQI>

Ferramenta útil:
```shell
cargo install cargo-watch

# agora conseguimos usar
cargo watch -x run
```

- Tipagem forte.
- Na declaração ocorre inferência de tipo.
- Por padrão as variáveis são imutáveis
    - Se quiser variável mutável, use `mut`
- Coding style: snake_case

```rust
// hours será do tipo inteiro
let hours = 30;

// se quiser mutável, precisa usar 'mut'
let mut counter = 0;
```

É possível recriar uma variável sem problema algum:
```rust
fn main() {
  let hours = 30;
  // do something...
  
  let hours = "quarenta";
  // this 👆 is perfectly fine
}
```

Definindo constantes:
```rust
// coding convention: ALL_CAPS_SNAKE_CASE
const SECONDS_IN_MINUTES: u32 = 60
```

Observações sobre constantes:

- precisa definir o tipo
- não pode ser definida novamente