# DiplomaDigital
Modelo conceitual das relações do diploma digital brasileiro

Este repositório disponibiliza o modelo conceitual completo das relações do diploma digital brasileiro. O modelo foi elaborado a partir da análise dos documentos normativos e técnicos e dos esquemas XSD da versão 1.05, tendo como principal referência o arquivo leiauteDiplomaDigital_v1.05.xsd. Sua finalidade é explicitar entidades, tipos, atributos, relações, restrições e cardinalidades associados à emissão, ao registro e à verificação do diploma digital.

# Principais encadeamentos

O núcleo do modelo é organizado por TInfDiploma, estrutura que reúne as informações centrais do diploma e estabelece os vínculos com os diferentes fluxos representados. A partir desse núcleo, destacam-se os seguintes encadeamentos:

Documento e núcleo informacional: TDiploma → TInfDiploma. Esse encadeamento relaciona o documento digital à estrutura responsável por organizar suas informações e dependências principais.

Dados do diploma: TInfDiploma relaciona-se com TDadosDiploma, TDadosDiplomaNSF e TDadosDiplomaPorDecisaoJudicial. Essas estruturas representam as variações previstas para os dados de emissão e mantêm relações com o diplomado, o curso, a instituição emissora e os demais componentes exigidos em cada situação.

Dados do registro: TInfDiploma também se relaciona com TDadosRegistro, TDadosRegistroNSF e TDadosRegistroPorDecisaoJudicial. Esses tipos organizam as informações referentes à instituição registradora, ao livro de registro e aos elementos necessários à identificação e à rastreabilidade do registro acadêmico.

Diplomado, curso e instituição emissora: os dados do diploma articulam TDadosDiplomado, TDadosCurso e TDadosIesEmissora, além das variações específicas previstas nos esquemas. Esse encadeamento representa a relação entre o titular do diploma, a formação concluída e a instituição responsável por sua emissão.

Instituição registradora e livro de registro: os dados de registro relacionam-se com TDadosIesRegistradora, TLivroRegistro e TLivroRegistroNSF. Essas relações organizam os elementos institucionais e documentais utilizados para registrar e individualizar o diploma.

Situações decorrentes de decisão judicial: TDadosDiplomaPorDecisaoJudicial e TDadosRegistroPorDecisaoJudicial incorporam relações com informações e declarações referentes ao processo judicial. Esses elementos distinguem esse fluxo das demais formas de emissão e registro previstas no modelo.

Assinatura e segurança: as estruturas de diploma e registro relacionam-se com o módulo TAssinantes e com o componente TSeguranca. Esse encadeamento reúne os elementos empregados na identificação dos responsáveis e na representação dos requisitos de assinatura e segurança do documento digital.

Em conjunto, esses encadeamentos tornam explícita a organização estrutural encontrada nos esquemas XSD e permitem acompanhar como as informações acadêmicas, institucionais, registrais e documentais se relacionam. As setas e cardinalidades do diagrama devem ser interpretadas como representação das relações e restrições identificadas durante a conceitualização do domínio.

O modelo constitui uma síntese conceitual e estrutural do recorte analisado. Portanto, não corresponde a uma ontologia operacional implementada, não apresenta formalização em RDF ou OWL e não demonstra que a interoperabilidade semântica entre sistemas tenha sido efetivamente alcançada. Sua contribuição consiste em oferecer uma base explícita e rastreável para etapas posteriores de formalização, implementação e validação.
