---
title: Misez votre ETH de manière individuelle
description: Un aperçu de la façon de commencer à miser votre ETH de manière individuelle
lang: fr
template: staking
emoji: ":money_with_wings:"
image: ../../../../../assets/staking/leslie-solo.png
alt: Leslie le rhinocéros sur sa puce d'ordinateur.
sidebarDepth: 2
summaryPoints:
  - Recevez un maximum de récompenses directement à partir du protocole (notamment les frais non brûlés après la Fusion) pour maintenir votre validateur en ligne et en bon fonctionnement
  - Faites fonctionner votre propre matériel et contribuez ainsi à la sécurité et la décentralisation du réseau Ethereum
  - Supprimez le tiers de confiance et gardez en permanence le contrôle sur vos fonds
---

## Qu'est-ce que la mise en jeu individuelle ? {#what-is-solo-staking}

La mise en jeu individuelle consiste à [faire fonctionner un noeud Ethereum](/run-a-node/) connecté à Internet et à déposer 32 ETH pour activer un [validateur](#faq), vous donnant la possibilité de participer directement au consensus du réseau.

Un nœud Ethereum est constitué à la fois d'un client de couche d'exécution (EL) et d'un client de consensus (CL). Ces clients sont des logiciels qui se coordonnent, avec un ensemble valide de clés de signature, pour vérifier les transactions et les blocs, attester de la tête de la chaîne, agréger les attestations et proposer des blocs.

Les validateurs individuels sont responsables du fonctionnement du matériel nécessaire à l'exécution de ces clients. Pour cela, il est fortement recommandé d'utiliser une machine dédiée que vous opérez depuis chez vous - c'est extrêmement bénéfique pour la santé du réseau.

Un validateur individuel reçoit des récompenses directement du protocole pour le maintien de son validateur en bon état de fonctionnement et en ligne.

## Pourquoi miser de manière individuelle ? {#why-stake-solo}

La mise en jeu individuelle demande plus de responsabilités, mais vous donne un contrôle maximal sur vos fonds et votre configuration de mise en jeu.

<CardGrid>
  <Card title="Gagnez de l'ETH frais" emoji="💸">
    Gagnez des récompenses en ETH, directement à partir du protocole lorsque votre validateur est en ligne, sans verser de commission à un quelconque intermédiaire.
  </Card>
  <Card title="Contrôle total" emoji="🎛️">
    Gardez vos propres clés. Choisissez la combinaison des clients et du matériel qui vous permet de minimiser vos risques et de contribuer au mieux à la santé et à la sécurité du réseau. Les services tiers de mise en jeu prennent ces décisions pour vous, et ils ne font pas toujours les choix les plus sûrs.
  </Card>
  <Card title="Sécurité du réseau" emoji="🔐">
    La mise en jeu individuelle est la façon la plus efficace de miser. En exécutant un validateur sur votre propre matériel depuis votre domicile, vous renforcez la solidité, la décentralisation et la sécurité du protocole Ethereum.
  </Card>
</CardGrid>

## Considérations avant de miser de manière individuelle {#considerations-before-staking-solo}

Bien que nous souhaitions que la mise en jeu individuelle soit accessible et sans risque pour tout le monde, la réalité est différente. Diverses considérations pratiques et sérieuses sont à garder à l'esprit avant de choisir de miser vos ETH de manière individuelle.

<InfoGrid>
  <ExpandableCard title="Lecture nécessaire" eventCategory="SoloStaking" eventName="clicked required reading">
    Lorsque vous opérerez votre propre nœud, vous devrez passer du temps à apprendre à utiliser le logiciel que vous avez choisi. Cela implique de lire la documentation adéquate et d'être connecté aux canaux de communication de ses équipes de développeurs.
    Mieux vous comprendrez le logiciel que vous exécutez et comment la preuve d'enjeu fonctionne, moins ce sera risqué pour vous, et plus il vous sera facile de résoudre toute sorte de problèmes qui peuvent survenir en tant qu'opérateur de nœud. 
  </ExpandableCard>
  <ExpandableCard title="Aisance en informatique" eventCategory="SoloStaking" eventName="clicked comfortable with computers">
    La configuration des nœuds nécessite un niveau d'aisance raisonnable dans le travail avec des ordinateurs, bien que de nouveaux outils apparaissent au fil du temps pour rendre cela plus facile. Comprendre l'interface de ligne commande est utile, mais n'est plus strictement nécessaire.
    Il faut également faire un petit peu de configuration matérielle et posséder une certaine compréhension des spécifications minimales recommandées.
  </ExpandableCard>
  <ExpandableCard title="Gestion des clés sécurisée" eventCategory="SoloStaking" eventName="clicked secure key management">
    Tout comme la façon dont les clés privées sécurisent votre adresse Ethereum, vous devrez générer des clés spécifiques pour votre validateur. Il est important de bien comprendre comment protéger les phrases de récupération ou les clés privées, et comment les stocker en toute sécurité.
    <p style={{marginTop: "1rem"}}><a href="/security">Sécurité d'Ethereum et prévention des arnaques</a></p>
  </ExpandableCard>
  <ExpandableCard title="Pas de retrait (pour l'instant)" eventCategory="SoloStaking" eventName="clicked no withdrawing">
    Il n'est pour l'instant pas possible de retirer les ETH misés ou les récompenses du solde d'un validateur. Le support des retraits est prévu pour la mise à niveau de Shanghai qui suivra La Fusion. Vous devriez vous attendre à ce que vos ETH soient immobilisés pendant au moins un à deux ans. Après la mise à niveau de Shanghai, vous pourrez retirer librement une partie ou la totalité de vos ETH mis en jeu.
  </ExpandableCard>
  <ExpandableCard title="Maintenance" eventCategory="SoloStaking" eventName="clicked maintenance">
    Le matériel tombe parfois en panne, tout comme les connexions réseau, et les logiciels client ont parfois besoin d'être mis à jour. La maintenance des nœuds est inévitable et nécessitera occasionnellement votre attention. Il est préférable de se tenir au courant de toutes les mises à niveau du réseau prévues, ou d'autres mises à jour critiques des logiciels client.
  </ExpandableCard>
  <ExpandableCard title="Disponibilité fiable" eventCategory="SoloStaking" eventName="clicked reliable uptime">
    Vos récompenses sont proportionnelles au temps passé par votre validateur en ligne et au fait qu'il atteste correctement. Tout temps passé hors ligne s'accompagne de pénalités proportionnelles au nombre de validateurs qui se trouvent hors ligne au même moment, mais <a href="#faq">ne donne pas lieu à des sanctions de délestage (slashing)</a>. La bande passante est également un facteur important, car les récompenses sont réduites pour les attestations qui ne sont pas reçues à temps. Les exigences varient, mais un minimum de 10 Mbit/s est recommandé (débits descendant et montant).
  </ExpandableCard>
  <ExpandableCard title="Risque de sanctions (délestage)" eventCategory="SoloStaking" eventName="clicked slashing risk">
    Les <em>sanctions de délestage (slashing)</em> diffèrent des pénalités d'inactivité (applicables si un validateur est hors ligne). Ce sont des pénalités bien plus graves, réservées aux délits ayant un caractère malveillant. Exécuter un client minoritaire en ayant vos clés chargées sur un seul appareil à la fois permet de minimiser le risque de délestage. Cela étant dit, toute personne plaçant des ETH doit être consciente du risque de délestage.
    
    <p><a href="https://medium.com/prysmatic-labs/eth2-slashing-prevention-tips-f6faa5025f50/">En savoir plus sur le délestage et le cycle de vie du validateur</a></p>
  </ExpandableCard>
</InfoGrid>

<StakingComparison page="solo" />

## Fonctionnement {#how-it-works}

<StakingHowSoloWorks />

Si vous le désirez, vous pouvez vous retirer en tant que validateur, ce qui élimine l'obligation d'être en ligne et met fin à toute autre récompense. Sachez que jusqu'à ce que la mise à jour planifiée de Shanghai, il ne sera pas possible de _retirer_ ces fonds.

Après Shanghai, les utilisateurs pourront retirer leurs récompenses ainsi que leur mise en jeu s'ils le souhaitent.

## Commencer avec la plateforme de lancement de la mise en jeu {#get-started-on-the-staking-launchpad}

La plateforme de lancement de la mise en jeu est une application open source qui vous aidera à devenir un validateur. Elle vous guidera dans le choix de vos clients, génèrera vos clés et déposera vos ETH dans le contrat de dépôt des mises en jeu. Une liste de vérification est fournie pour vous assurer que vous avez fait le tour de la question pour installer votre validateur en toute sécurité.

<StakingLaunchpadWidget />

<InfoBanner emoji=":panda:" isWarning>
<strong>Note pour les validateurs actuels :</strong> La Fusion approche, ce qui apporte quelques changements depuis le lancement de la mise en jeu. Assurez-vous que vous êtes bien préparé avec la <a href="https://launchpad. ethereum. org/en/merge-readiness">liste de vérification de la Fusion</a> sur la plateforme de lancement de la mise en jeu.
</InfoBanner>

## Éléments à prendre en compte avec les outils de configuration de nœud et de client {#node-tool-considerations}

Un nombre croissant d'outils et de services vous aident à miser vos ETH, mais chacun comporte des risques et des avantages différents.

Les indicateurs d'attributs sont utilisés ci-dessous pour signaler des forces ou faiblesses notables d'un outil de mise en jeu répertorié. Utilisez cette section comme référence pendant que vous choisissez les outils qui vous aideront dans votre parcours de mise en jeu.

<StakingConsiderations page="solo" />

## Explorer les outils de configuration de noeud et de client {#node-and-client-tools}

Il existe une variété d'options disponibles pour vous aider dans votre configuration. Utilisez les indicateurs ci-dessus pour vous guider à travers les outils ci-dessous.

<InfoBanner emoji="⚠️" isWarning>
Veuillez noter l'importance de choisir un <a href="/developers/docs/nodes-and-clients/client-diversity/">client minoritaire</a> , car cela améliore la sécurité du réseau et limite vos risques. Les outils qui permettent de configurer un client minoritaire sont désignés comme <em style="text-transform: uppercase;">"multi-client."</em>
</InfoBanner>

#### Outils de nœud

<StakingProductsCardGrid category="nodeTools" />

#### Générateurs de clés

Ces outils peuvent être utilisés en alternative à [l'interface de dépôt de mise en jeu](https://github.com/ethereum/staking-deposit-cli/) pour vous aider à générer vos clés.

<StakingProductsCardGrid category="keyGen" />

Vous souhaitez suggérer un outil de mise en jeu que nous avons manqué ? Consultez notre [politique de liste de produits](/contributing/adding-staking-products/) pour voir s'il conviendrait, et le soumettre à examen.

## Explorer les guides de mise en jeu individuelle {#staking-guides}

<StakingGuides />

## FAQ {#faq}

Voici quelques-unes des questions les plus fréquentes relatives à la mise en jeu qui valent la peine d'être connues.

<ExpandableCard title="Qu'est-ce qu'un validateur ?">
Un <em>validateur</em> est une entité virtuelle qui vit sur la Chaîne phare et participe au consensus du protocole Ethereum. Les validateurs sont représentés par un solde, une clé publique et d'autres propriétés. Un <em>client de validateur</em> est le logiciel qui agit au nom du validateur en détenant et en utilisant sa clé privée. Un même client peut contenir plusieurs paires de clés, contrôlant de nombreux validateurs.
</ExpandableCard>

<ExpandableCard title="Puis-je déposer plus de 32 ETH ?">
Chaque paire de clés associée à un validateur nécessite exactement 32 ETH pour être activée. Déposer plus d'ETH sur un même ensemble de clés n'augmente pas le potentiel de récompense, car chaque validateur est limité à un <a href="https://www.attestant.io/posts/understanding-validator-effective-balance/">solde effectif</a> de 32 ETH. Cela signifie que la mise en jeu se fait par tranches de 32 ETH, chacune avec son propre jeu de clés et son propre solde.

Ne déposez pas plus de 32 ETH pour un seul validateur. Cela n'augmentera pas vos récompenses, et ils seront verrouillés jusqu'à la mise à jour de Shanghai.

Si la mise en jeu individuelle vous semble trop exigeante, envisagez d'utiliser un <a href="/staking/saas/">fournisseur de mise en jeu en tant que service</a>, ou si vous possédez moins de 32 ETH, consultez <a href="/staking/pools/">les groupes d'enjeu</a>.
</ExpandableCard>

<ExpandableCard title="Vais-je être sanctionné si je me déconnecte ? (tdlr : Non.)">
Se déconnecter pendant que le réseau se finalise correctement n'entraînera PAS de délestage. De petites <em>pénalités d'inactivité</em> sont encourues si votre validateur n'est pas disponible pour attester pendant une période donnée (d'une durée de 6,4 minutes chacune), mais cela reste très différent du <em>délestage</em>. Ces pénalités sont légèrement inférieures à la récompense que vous auriez obtenue si le validateur avait été disponible pour attester, et les pertes peuvent être récupérées avec un temps de remise en ligne à peu près équivalent.

Notez que les pénalités d'inactivité sont proportionnelles au nombre de validateurs se trouvant hors ligne en même temps. Dans les cas où une grande partie du réseau est hors ligne en même temps, les pénalités pour chacun de ces validateurs seront plus importantes que lorsqu'un seul validateur est indisponible.

Dans des cas extrêmes, si le réseau cesse de se finaliser parce que plus d'un tiers des valideurs sont hors ligne, ces utilisateurs subiront ce que l'on appelle une <em>fuite d'inactivité quadratique</em>, qui consiste en une fuite exponentielle d'ETH à partir de comptes de valideurs hors ligne. Cela permet au réseau de s'auto-régénérer en brûlant les ETH des validateurs inactifs jusqu'à ce que leur solde atteigne 16 ETH, après quoi ils seront automatiquement éjectés du pool de validateurs. Les validateurs en ligne restants comprendront finalement, à nouveau, 2/3 du réseau, satisfaisant ainsi la supermajorité nécessaire pour finaliser à nouveau la chaîne.
</ExpandableCard>

<ExpandableCard title="Comment être sûr de ne pas subir de délestage ?">
Pour faire court, cela ne peut jamais être totalement garanti, mais si vous êtes de bonne foi, que vous utilisez un client minoritaire et que vous ne conservez vos clés de signature que sur une seule machine à la fois, le risque de subir un délestage est quasiment nul.

Seuls quelques moyens spécifiques peuvent aboutir à ce qu'un validateur soit délesté et éjecté du réseau. À l'heure où nous écrivons ces lignes, les délestages qui se sont produits sont exclusivement le produit de configurations matérielles redondantes où les clés de signature sont stockées sur deux machines distinctes à la fois. Cela peut entraîner par inadvertance un <em>double vote</em> de vos clés, ce qui constitue une faute sanctionnable.

L'exécution d'un client supermajoritaire (tout client utilisé par plus de 2/3 du réseau) comporte également le risque d'un délestage dans le cas où ce client présente un bogue qui entraîne une fouche de la chaîne. Cela peut aboutir à une fourche défectueuse qui sera finalisée. Pour revenir à la chaîne voulue, il faudrait soumettre un <em>vote circulaire</em> en essayant d'annuler un bloc finalisé. Il s'agit également d'une infraction passible de sanctions et peut être évité simplement, en utilisant, à la place, un client minoritaire.

Des bogues équivalents dans <em>un client minoritaire ne seraient jamais finalisés</em> et ne donneraient donc jamais lieu à un vote circulaire, et entraîneraient simplement des pénalités d'inactivité, et <em>non un délestage</em>.

<p><a href="https://hackernoon.com/ethereums-client-diversity-problem">En savoir plus sur l'importance d'exploiter un client minoritaire.</a></p>
<p><a href="https://medium.com/prysmatic-labs/eth2-slashing-prevention-tips-f6faa5025f50">En savoir plus sur la prévention du délestage</a></p>
</ExpandableCard>

<ExpandableCard title="Quel est le meilleur client ?">
Les clients individuels peuvent varier légèrement en termes de performances et d'interface utilisateur, car ils sont tous développés par des équipes différentes utilisant des langages de programmation variés. Ceci étant dit, aucun d'entre eux n'est "le meilleur". Tous les clients de production sont d'excellents logiciels, qui exécutent tous les mêmes fonctions de base pour se synchroniser et interagir avec la blockchain.

Puisque tous les clients de production fournissent les mêmes fonctionnalités de base, il est en fait très important que vous choisissiez un <strong>client minoritaire</strong>, c'est-à-dire tout client qui n'est actuellement PAS utilisé par une majorité de valideurs sur le réseau. Cela peut sembler paradoxal, mais le fait d'utiliser un client majoritaire ou supermajoritaire vous expose à un risque accru de délestage en cas de bogue dans ce client. Utiliser un client minoritaire limite considérablement ces risques.

<a href="https://mirror.xyz/jmcook.eth/S7ONEka_0RgtKTZ3-dakPmAHQNPvuj15nh0YGKPFriA">En savoir plus sur les raisons pour lesquelles la diversité des clients est essentielle</a>
</ExpandableCard>

<ExpandableCard title="Puis-je simplement utiliser un VPS (serveur privé virtuel) ?">
Bien qu'un serveur privé virtuel (VPS) puisse être utilisé en remplacement du matériel domestique, l'accès physique et l'emplacement de votre client validateur <em>ont leur importance</em>. Les solutions centralisées dans le cloud, telles que Amazon Web Services ou Digital Ocean, offrent la commodité de ne pas avoir à obtenir et à faire fonctionner du matériel, au détriment de la centralisation du réseau.

Plus il y a de clients validateurs fonctionnant sur une seule solution de stockage en cloud centralisée, plus cela devient dangereux pour ces utilisateurs. Tout événement qui mettrait ces fournisseurs hors ligne, qu'il s'agisse d'une attaque, d'une demande réglementaire ou d'une simple panne de courant ou d'Internet, entraînera la mise hors ligne simultanée de tous les clients de validation qui dépendent de ce serveur.

Les pénalités hors ligne sont proportionnelles au nombre de personnes se trouvant hors ligne au même moment. L'utilisation d'un VPS augmente considérablement le risque de voir les pénalités hors ligne devenir plus sévères, et accroît votre risque de fuite quadratique ou de délestage dans le cas où la panne serait suffisamment importante. Pour minimiser vos propres risques et ceux encourus par le réseau, les utilisateurs sont fortement encouragés à se procurer et à exploiter leur propre matériel.

<a href="https://consensys.net/blog/codefi/rewards-and-penalties-on-ethereum-20-phase-0/">En savoir plus sur les récompenses et les pénalités</a>
</ExpandableCard>

<ExpandableCard title="Dois-je faire quelque chose avant la Fusion ?">
Les validateurs exécutant actuellement un client de la couche de consensu (Beacon Chain) devront également exécuter un client de la couche d'exécution après la Fusion. La nouvelle API Moteur sera utilisée pour interagir entre les deux couches, et nécessitera un JWT secret. Si vous faites actuellement tourner la Beacon Chain (consensus) sans un client de la couche d'exécution, vous devrez synchroniser la couche d'exécution avant la Fusion pour rester synchronisé avec le réseau.

La Fusion apportera également des frais de transaction non brûlés aux validateurs. Ces frais ne s'accumulent pas dans le solde associé aux clés de validation, mais peuvent être dirigés vers une adresse Ethereum ordinaire de votre choix. Pour recevoir vos tips (frais de priorité) sur les blocs proposés, vous devez mettre à jour les paramètres de votre client avec l'adresse vers laquelle vous souhaitez que ces frais soient envoyés.

Des liens vers la documentation de chaque client et des informations supplémentaires peuvent être trouvés dans la liste de vérification de la préparation à la Fusion sur la plateforme de lancement.

<ButtonLink to="https://launchpad.ethereum.org/merge-readiness/">
Fusionner la liste de vérification de la disponibilité
</ButtonLink>
</ExpandableCard>

## Complément d'information {#further-reading}

- [Ethereum's Client Diversity Problem](https://hackernoon.com/ethereums-client-diversity-problem) - _@emmanuelawosika 2022_
- [Helping Client Diversity](https://www.attestant.io/posts/helping-client-diversity/) - _Jim McDonald 2022_
- [Client diversity on Ethereum's consensus layer](https://mirror.xyz/jmcook.eth/S7ONEka_0RgtKTZ3-dakPmAHQNPvuj15nh0YGKPFriA) - _jmcook.eth 2022_
- [How To: Shop For Ethereum Validator Hardware](https://www.youtube.com/watch?v=C2wwu1IlhDc) - _EthStaker 2022_
- [Step by Step: How to join the Ethereum 2.0 Testnet](https://kb.beaconcha.in/guides/tutorial-eth2-multiclient) - _Butta_
- [Eth2 Slashing Prevention Tips](https://medium.com/prysmatic-labs/eth2-slashing-prevention-tips-f6faa5025f50) - _Raul Jordan 2020_
- [Rewards and Penalties on Ethereum 2.0](https://consensys.net/blog/codefi/rewards-and-penalties-on-ethereum-20-phase-0/) - _James BeckMarch 2020_
