---
## Exercício `Agenda`

Crie um repositório baseado [neste template](https://github.com/ermogenes/agenda-template).

Crie um banco de dados com a estrutura contida no arquivo `scripts/agenda.sql`:

```sql
DROP SCHEMA IF EXISTS `agenda` ;
CREATE SCHEMA IF NOT EXISTS `agenda` DEFAULT CHARACTER SET utf8 ;
USE `agenda` ;
DROP TABLE IF EXISTS `contato` ;
CREATE TABLE IF NOT EXISTS `contato` (
  `id` INT NOT NULL AUTO_INCREMENT,
  `nome` VARCHAR(50) NOT NULL,
  `fone` VARCHAR(20) NULL,
  `estrelas` INT NULL,
  PRIMARY KEY (`id`),
  UNIQUE INDEX `nome_UNIQUE` (`nome` ASC) VISIBLE)
ENGINE = InnoDB;
```

Implemente as funções indicadas no menu, salvando no banco de dados criado.

---
