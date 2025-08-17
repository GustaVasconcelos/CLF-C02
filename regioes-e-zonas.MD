# Regiões e Zonas de Disponibilidade na AWS

## Região
- Uma **região** é um **conjunto geográfico** onde a AWS mantém sua infraestrutura.  
- Cada região é **independente** das demais (por exemplo: `us-east-1` na Virgínia, `sa-east-1` em São Paulo).  
- Dentro de uma região existem **múltiplas zonas de disponibilidade**.  
- Ao escolher uma região, você define onde seus dados e serviços serão **armazenados e processados**.  

## Zona de Disponibilidade (Availability Zone - AZ)
- Uma **zona de disponibilidade** é formada por **um ou mais data centers físicos** dentro de uma região.  
- Cada AZ tem sua própria **energia, refrigeração e conectividade**.  
- As AZs de uma mesma região são interconectadas com **links de baixa latência**.  
- Isso permite criar sistemas **altamente disponíveis**, replicando recursos em diferentes AZs.  

## Como funciona na prática
- Se você hospeda sua aplicação em apenas **uma AZ**, ela pode ficar indisponível caso ocorra uma falha.  
- Se você replica sua aplicação em **duas ou mais AZs da mesma região**, ela continua funcionando mesmo que uma AZ apresente problemas.  
- Exemplo: Região **São Paulo (`sa-east-1`)** possui **três AZs**: `sa-east-1a`, `sa-east-1b`, `sa-east-1c`.  

---

## Resumindo
- **Região** = Área geográfica (ex.: Brasil, EUA, Europa).  
- **Zona de Disponibilidade** = Data centers **redundantes** dentro da região.  

## Quantas zonas existem em uma região?

- Cada **região AWS** possui **no mínimo 2 zonas de disponibilidade (AZs)**.  
- A maioria das regiões possui **3 ou mais AZs**.  
- Isso garante que os clientes possam **replicar aplicações** e manter **alta disponibilidade**.  
- As AZs são **fisicamente separadas**, mas interligadas com **baixa latência**.  
