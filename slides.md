slidenumbers: true
footer: Carlos Becker - Codecon Summit 2025
slide-transition: fade(0.5)
theme: Plain Jane

# [fit] Building GoReleaser

## [fit] from shell script to paid product

![](./presentation2.png)

^ oi! estou muito feliz de estar aqui hoje, e espero que isso seja interessante para vocês

---

# $ whoami

Carlos Alexandro Becker

- `@caarlos0` most places
- works `@charmbracelet`
- maintains `@goreleaser`
- [`caarlos0.dev`](https://caarlos0.dev)

![fit right](./carlos-and-bash.png)

^ não sou influencer, então esse sou eu e meu cachorro, bash.
trabalho, coisas de oss, site com redes sociais

---

# Agenda

1. What is GoReleaser
1. The Lore
1. Lessons learned
1. The Future

^ o que planejei para hoje é explicar rapidamente o que é o goreleaser, contar como chegou onde está hoje, compartilhar algumas coisas que aprendi, algumas das quais são talvez um pouco contra-intuitivas, e os planos para o futuro.
não é a história enfeitada pra pegar view no instagram, e sim coisas reais que aconteceram, tanto boas quanto as ruins

---

# GoReleaser

- Release automation tool
- Build, package, sign, publish, announce
- Configurable through a `.yaml` file
- Nudges you into doing the _"right thing"_
- Supports Go, Rust, Zig, Python, and TypeScript
- [goreleaser.com](https://goreleaser.com)

![fit right](./goreleaserfundo.png)

---

# The Lore

![](./presentation2.png)

---

## 2015: The beginning

- I was working on one of my Go projects
- Created a [`release.sh`](https://github.com/getantibody/antibody/commit/5d06dae0c78d1655fc243183f96d8a0a7a3cc197)
- Didn't think anything of it
- Same as thousands before

![fit right](much.png)

^ começa meio que por acidente.
Eu estava apenas aprendendo go, e tinha um projeto paralelo.
Criei um shell script pra resolver meu problema.
Não era nada especial, apenas um script shell, como muitos antes dele, e muitos depois dele
por alguns meses não pensei mais nisso, meu shell funcionava.

---

## 2016: Rewrite in Go

- I now have a dozen of Go projects
- Moved that script into its [own repository](https://github.com/getantibody/antibody/commit/5d06dae0c78d1655fc243183f96d8a0a7a3cc197)
- Doing OSS during EOY holidays, needed more features
- Rewrote it in Go
- Shared it online, and people liked it!

^ Agora com mais projetos, todos eles precisam de releases
Movi pra um repo proprio, configs via `--flags`. Era ruim, mas resolveu o problema por mais alguns meses.
Ja em dezembro, nas ferias de final de ano, ao inves de ficar de boa, tava eu la codando.
"Preciso do Homebrew" "Vai ser ruim fazer isso com bash..." "Vou transformar isso num projeto Go!"
compartilhei online, e para minha surpresa as pessoas gostaram!

---

## 2017: Spreading the word

- Kept adding features to it
- Wife drew the mascot/logo
- Using it in all my Go projects
- Talking about it in local Meetups
- \>1k stars

![fit right](./goreleaserfundo.png)

^ percebi que tinha criado um projeto mais legal do que achei que seria.
conforme crescia em popularidade, continuei adicionando mais recursos, minha esposa desenhou um mascote, e comecei a falar sobre isso em alguns meetups locais em joinville
no final do ano já tinha mais de 1k stars

---

## 2018: Burning out

- Created nFPM & OpenCollective
- \>1k public repositories using it
- More meetups & _Gophercon Brazil_
- Refactored core to support multiple languages, eventually
- \>3k stars
- Burnout

^ 2018 eu trabalhei pra baralho.
criei o nfpm, o primeiro projeto derivado, e criei a pag no OpenCollective, ja com algumas empresas legais doando, e ainda está ativo hoje.
falei em mais meetups, e na gophercon brasil.
queria suportar múltiplas linguagens como plugins, deixei meio pronto achando que suporte iria melhorar no Go - o que nunca aconteceu.
1k repos baseado na busca do github. e 3k stars
burnout: se você constantemente se pergunta se está em burnout ou não, pode valer a pena verificar. Além disso, se seu parceiro diz que você trabalha demais, provavelmente está certo
ainda não me sinto muito confortável falando sobre isso, mas escrevi um pouco mais sobre isso, link vai estar no final dos slides.

---

## 2019 & 2020: Recovering and COVID

- Recovering from burnout
- Planning v1.0.0
- \>5k stars

^ basicamente 2019 tentei me recuperar do burnout.
Mudei de emprego, melhorei rotina de exercício, cortei álcool, comendo mais limpo
também comecei a falar sobre e planejar uma v1, mas estava principalmente apenas indo com a mare pela maior parte do ano

---

![](./wth.gif)

^ quer dizer, 2020 é basicamente um borrão, nem lembro da maior parte
mas FWIW, terminei 2020 muito melhor de saude fisicamente e mentalmente.

---

## 2021: We are SO back!

- _GoTime_ Podcast
- Launched **v1.0.0!** 🎉
- GitHub Sponsors
- **GoReleaser Pro**
- \>9k stars

^ gotime: estar num podcast desse calibre era algo que o jovem eu nunca sonharia. pareceu uma grande conquista, especialmente considerando que venho de uma família simples do interior do brasil.
estava no primeiro lote a ter sponsors habilitado no brasil, ou talvez SA, não lembro ao certo. Mas foi massa.
sponsors deram algum dinheiro, mas não parecia que algum dia seria sustentável, me parece geralmente mais relacionado à "fama" do que qualquer outra coisa
então, para tentar tornar as coisas sustentáveis, lancei o goreleaser pro, uma versão paga com recursos extras.
confesso, achei que não funcionaria, e se não funcionasse, provavelmente teria parado de investir tanto tempo no projeto.
para minha surpresa, funcionou! e agora a diversão real começa

---

## 2022: Full-time open source

- Working at Charm, doing OSS all day long
- Split & Merge, `--nightly`, AUR
- Proper release announcements
- \>10k stars

^ comecei a trabalhar na charm, fazendo principalmente dev tooling oss lá.
era meu sonho uma decada antes, e agora meio que por cagada to aqui.
enfim, continuei trabalhando nas coisas, como split e merge, nightly builds, e mais.
também passamos a 10k estrelas

---

## 2023: More professional

- Proper [release cadence](https://goreleaser.com/blog/release-cadence/#thank-you-notes)
- Ko, health check, upx, nix, Winget
- \>12k stars

^ pelo final 2022 já estava seguindo mais ou menos 1 feature release por mês, mas em 2023 tornei isso oficial.
também documentei adequadamente quais versões são suportadas na versao free e pro, etc etc.
finalmente, adicionei diversos recursos novos, como Ko, upx, nix, winget, e mais
e passamos de 12k estrelas

---

## 2024: At last, multiple languages

- Launched **v2.0.0** 🎉
- Rust and Zig support!
- DMG, MSI, macOS notary, App Bundles,
- \>14k stars
- \>100 pro customers

![right](./mascots.png)

^ finalmente, lancei a v2, e então, graças a meu amigo Raphael que ficou me cobrando, finalmente adicionei suporte a Rust e Zig.
Rio term é a primeira "aplicação real" usando goreleaser com rust, btw.
Também adicionei mais coisas relacionadas a aplicações desktop, ex. dmg, msi, notarização, app bundles, etc.
Levou anos para passar dos 100 clientes - mas neste ponto, finalmente parece um negócio viavel. tldr: eu poderia nao ter mais emprego.

---

## 2025: Moving forward

- Bun, Deno, Poetry, and UV support
- AI changelog, MCP server, NPM, Casks
- _Cup o' Go_ and _Fallthrough_ Podcasts
- Better support for desktop apps
- \~200 customers, \~15k stars
- _Codecon Summit_ 🙃

^ o que nos traz para 2025, o ano do linux no desktop. estamos jogando em handhelds arch linux e a AI vai substituir todo mundo 3 meses atras, what a time to be alive
bem, por enquanto adicionei suporte a python com uv e poetry e typescript com bun e deno.
coloquei como meta este ano falar em duas conferências, esta é a segunda! também fui em 2 podcasts até agora falar sobre go e goreleaser
GoReleaser Pro agora tem 200 clientes pagantes, e um MRR muito bom. Falando em dinheiro brasileiro, paga mais que meu último emprego como SRE sênior no Brasil.
Super feliz com isso!

---

# Lessons learned

![](./presentation2.png)

^ bem, agora para alguns dos erros que cometi ao longo dos anos, e o que aprendi.

---

## Boring software

- People want _predictability_ instead of _novelty_ when releasing their software
- Boring is _predictable_
- _Boring is good_, actually

^ pessoas não querem surpresas em algumas partes de suas vidas, elas querem estabilidade.
releases de software já são cheios de ansiedade como são, entao o software que faz isso deveria ser previsível.
software chato é previsível, essa é uma das razões pelas quais é chato.
software chato é bom, na verdade, na maioria das vezes.
todo mundo quer trabalhar no que é legal agora, mas software chato roda a maior parte da infraestrutura, e provavelmente vai continuar assim por muito tempo.
talvez seja só eu ficando velho, mas agora meio que gosto de software chato.

---

## Distribution

- Really hard, unless you are a _tech influencer_
- Creator and creation get conflated
- If you are a _tech influencer_, then you might have other problems

^ este é o problema mais difícil de resolver, e afaik não há solução mágica para isso, pois tem muito a ver com "vibes" e um tanto sorte.
marketing forcado no geral me parece que não funciona. não passa o vibe check, e a galera não curte.
ja posts criativos, memes, etc, parecem funcionar ok. vejam htmx no twitter por exemplo.
agora, se você conseguir que alguém famoso use e fale sobre seu proj, voce provavelmente consegue uma distribuicao boa
ainda sobre vibes, eu agora sou 'o cara do goreleaser', e tudo bem, é só algo pra ter em mente
Então o que eu digo pessoalmente também afeta a visão do meu produto, e vice-versa.
Ja se você é tech influencer, imagino que pode ter outros problemas: você provavelmente em algum momento vai perguntar se sua coisa está fazendo números porque é realmente boa, ou se é porque foi você quem fez. Provavelmente uma combinação de ambos.
Ex: vejam o pieter levels no twitter. Se ele fizesse o pudim.com.br em 3 dias ele estaria tirando 10k MRR com ads ou algo do tipo

---

## Naming things

- "it releases Go binaries, its a Go Releaser"

![inline](./gore_leaser_2.png)

^ escolhi o nome depois de pensar sobre isso por uns 5 segundos.
não percebi que poderia ser lido errado até um bom tempo depois (meses, talvez um ano).

---

## Naming things

- "it releases Go binaries, its a Go Releaser"
- "gore leaser"
- mix up with `gorelease` (without the `r`)
- the **Go** prefix

![right](./gore_leaser.png)

^ eventualmente, se tornou meio que uma piada recorrente - com arte e tudo mais
gorelease sem o r do time de release do Go.
prefixo go meio que me prendeu por muito tempo, e aposto que estou perdendo novos usuários/clientes por causa disso ate hj
às vezes palavras perfeitamente normais em inglês soam como palavrão em outras línguas, ou vice versa, etc, etc etc
se você está fazendo algo que acha que pode ser algo grande, pense bem sobre o nome. facil pedir pro chatgpt hoje em dia pra fazer um check.
nomear coisas é difícil

---

## Pricing

- Harder than pricing physical products
- _Guess_ based on what you know and what you think it's worth
- Enterprises usually expect overcharging (legal, forms, etc)

^ produtos físicos você pode derivar o preço dos materiais mais mão de obra.
software você está basicamente permitindo acesso a ele, não vendendo algo.
no meu caso, nem há servidores, é só pagar pelo direito de usar recursos extras.
tldr não tenho nenhuma base de onde derivar um valor, alem das minhas horas de trabalho.
entao eh basicamente chute, mais ou menos informado, mas chute, especialmente de um POV que você não conhece.
trabalhei principalmente em empresas pequenas a médias, entao ja tinha uma nocao de preco nessas faixas, mas as realmente grandes são completamente diferentes.
muito juridiquês, docs, etc, talvez voce inclusive precise de um advogado - e elas esperam ser cobradas a mais por isso
então cobre a mais.

---

## Licensing

- MIT is probably too permissive
- Changing later might feel like bait-and-switch
- Consider changing it earlier rather than later

^ para melhor ou pior, sempre uso MIT, que é bem permissiva... talvez permissiva demais em muitos casos
todos já vimos: grandes corporações vendendo oss como serviço, esse tipo de coisa.
e acredito que nos, a comunidade em geral, somos parete do problema
se qualquer projeto oss meio grande muda a licença, todos reclamamos.
e também reclamamos se grandes corporações fazem coisas que poderiam ter sido prevenidas pela troca de license.
uma vez que você tem X popularidade , pessoas vão achar que foi bait and switch, não importa se teu software tem 10 anos ou 10 dias
você também não pode relicenciar contribuições passadas sem aprovação de quem contribuiu, e isso pode simplesmente não ser possível (ex. pessoas morrem)
enfim, pense sobre isso o mais cedo possível, se eu fosse começar algo que acho que pode ser muito bom, começaria com uma licença diferente, provavelmente - FSL foi aceita pela SPDX e tenta ser livre e sem free ride ao mesmo tempo. Veremos como roda isso ai

---

## Flexibility, Simplicity, and finding balance

- I love flexible software
- It leads to madness
- I hate flexible software
- Scope creep, accidental complexity

![right 140%](./seen-things.gif)

^ aqui eh mais sobre software em geral do que oss, mas eh algo que enfrentei muito no goreleaser
todo mundo gosta de software flexível. planilhas é um bom exemplo.
quanto mais flexível, mais doideira o povo faz, e como mantenedor, você vai receber tickets insanos que terá de entender pra ajudar seu usuário.
então, hoje antes de adicionar uma nova opcao, tento pensar sobre essa nova config em combinação com todas os outros ja existentes.
+- relacionado, sobre simplicidade o que aconteceu eh perdi um pouco do idealismo que tinah quando mais jovem.
é fácil falar de simplicidade em software novo e pequeno, mas eh dificil manter tudo "simples" num software velho e grande, no longo prazo.
você continua adicionando coisas, tem usuários agora, então nem sempre pode fazer da melhor forma porque pode ser uma mudança que quebra, ou demorar muito, então as coisas ficam complicadas.
você vai acabar com alguma complexidade acidental conforme o escopo cresce, dificil d+ fugir
a parte realmente difícil aqui é encontrar equilíbrio entre escopo, simplicidade, flexibilidade, e evitar breaking changes
e a dica que dou aqui eh: sabe qdo vc ta codando um negocio e te da uma vontade de fazer uma careta, ou vem aquela vozinha e fala "ta estranho isso ai"?
entao, pare, reflita sobre as coisas, vai caminhar um pouco, tomar um cafe, sei la... mas não seja muito reativo.
uns 90% de todas as cagadas que fiz em software foram coisas que fiz reativamente - ticket apareceu, queria resolver logo, fiz o que veio na ideia na hora, e a primeira ideia quase sempre eh ruim
enfim, escute seu instinto, está certo na maioria das vezes.

---

## Building products

- Side projects: for fun and studying
- Products: solving problems

^ esse ponto eh provavelmente obvio pra maioria, mas acho que especialmente pra quem ta comecando talvez não seja. entao aqui vai:
a maior parte dos projetos que crio, eu parto de um problema que eu tenho, e tento resolver esse problema.
vejo mta coisa por ai, especialmente agora com AI, que parece ser "ah eu queria usar X tech pra alguma coisa ai fiz isso aqui", e a regra eh isso não dar bom
claro, ainda tenho os projetinhos pra brincar com tech nova, aprender coisas, etc
mas se o objetivo eh fazer um projeto que outras pessoas vao efetivamente usar, as chances de sucesso costumam ser bem melhores se vc partir de um problema.

---

# The Future

![](./presentation2.png)

---

## The future

- Support more languages and distribution channels
- Improve docs, error messages, small feats, etc
- tl;dr keep working on it

^ meus planos para o futuro são boring :)
enfim, provavelmente vou adicionar mais linguagens e canais de distribuição, e continuar trabalhando em todo o resto
boring eu sei, igual meu slide sobre boring software :)

---

![](./presentation2.png)

# PS: I have stickers!

## Come chat and I'll give you some 😉

---

![](./thanks.gif)

^ bem, é isso que tenho para hoje, obrigado pela atenção. espero que tenham gostado. vlw!

---

# Links

- [caarlos0.dev](https://caarlos0.dev)
- [goreleaser.com](https://goreleaser.com)
- [carlosbecker.com/posts/codecon-goreleaser](https://carlosbecker.com/posts/codecon-goreleaser)
- [github.com/caarlos0/codecon-2025](https://github.com/caarlos0/codecon-2025)
