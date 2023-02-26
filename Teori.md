# algo-teori-sem3

## Grafet 
quajm bashkesin e kulmeve te cilat jane te lidhura me ane te segmenteve.

### Qka quaj rruge ne nje graf ?
Seri te kulmeve te lidhura me segmente .

### Qka quaj cikel ?
Cikel quajm kur  kulmi i pare dhe i fundit eshte i njejte.
Shpjego Ciklin e Ederit dhe Hamiltonit?
C.Ederit  perdor secilin segment saktsisht nje her.
C.Hamiltonit  perdor secilin kulm saktsisht nje her.

### Sa lloje te grafeve kemi ?
Directed dhe Undirected.

### Sa % kemi human error?
4% Human error.
Undirected Graph Anomalite:
Segmentimi paralel dhe ka self loop.
Perdor Symbol Table per konvertimin e emrave dhe integjereve.

### Cka jane MFormat Methods?
jane metoda per me i hek gabimet ne sisteme softwerike (makina vetlevizese tesla).

### Si emertohen kulmet e nje grafi ?
V-1

### Qysh me i lidh dy grafe me kod ?
Public class Graph
Graph(int V);
Graph(int W);
addEdge(int V,int W);

### Menyra e paraqitjes se grafeve?
1.Set Of Edges graph
2.Matric(E shpejt per searching)
3.Array List

### Mangesit e Matric Graph :
Double Data(shume vend ne memorie zen,smujna me bo segmentim paralel)

### A eshte me i shpejte nje graf me 200 a 2000 segmente .
2000 eshte me i shpejte.
Undirected add nkod:
adj[V].add[w]; 1-2
adj[W].add[V]; 2-1

### Cilet jane dy algoritmet per kerkim(searching):
DFS - ne stack (Lifo) ideja e saj eshte qe te mos e vizitoj nje kulm dy her prandaj e bon check,perdoret per kerkim randomly jo specific.
BFS - ne queue(FIFO) perdoret me shume kur kemi me bo searching dicka specifike

### Karakteristikat e DFS:
Impimentohet ne stack 
Shkon ne thellsi sa me shume qe eshte e mundur .

### Paraqitja e DFS?
V/edgeTo[]/marked
EdgeTo=me i lidh kulmet ne graf.
Marked=me kshyr a e kena vizitu .

### Karakteristikat e BFS?
Implimentohet me Query(fifo)
Shkon ne gjersi .

### Cili eshte me i shpejte DFS VS BFS?
Njejte.
Paraqitja e BFS ?
V/edgeTo[],distTo[];
distTo[]=me sa hapa ose segmente kemi mrri .

### Si ndahen Grafet ne baze te emertimit :
Te thjeshta dhe te perbera
List of Edges grapf mirmbahet me linked list ose array.
Adjacency-list mirmbahet me emrat e kulmeve array of lists.
DFS(Depth-first Search)-pershkrun grafin ne menyr sistematike.
Gjen dhe e largon Dead-Code.
Detekton infinite loop.
BFS(Breadth-fist Search)- perdor queue ,dhe i perserit queue deri sa vargu te jet empty(FIFO).
Perdor marked[],dhe id[].
Nje graf nuk ka cycle nese ne ate graf munesh me gjet Topological order.
BFS gjen rrugen me te shkurt te grafit.

### Connected components vs. strongly connected components
Connected Components  quajm kur komponentet kane nje rrug te komunikojn mes veti.(let mu perdor me DFS).
Strongly CC  quajm kur komponentet kan nje komunikim me drejtime qe mund te shkojn nga njeri tek tjetri.
Algoritmi me i mire per me perdor Strongly CC eshte Kisharaju.
Directed Graph  gati identik me graf API .
Per me u paraqit DiGraph perdoret adjacency list.
Kosaraju-Sharir algorithm  Komponentet Strong G jane te njejta si G ^R(reverse).Perdor DFS.
Implimentimi i lete dhe DFS perdor dyher pasi qe niher e ben reverse.

### Topological sort (DAG)  perdor DFS.
Me grafe punojm me sorttable.
Dead code  quajm kodin i cili gjindet ne program por nuk perdoret asnjeher.
3 menyra  me i paraqit grafet:
Array List
Set of Edges 
Matrice
Anomali  Paralel edges dhe self loop 
Paralel edges  kur nje graf ka nje lidhje me nje graf tjeter ose me shume se nje .
Self Loop 

### Directed  kur kan kahje segmentet

### Undirected-segmentet nuk kan kahje
Metoda me shtu segmente ose brinje  addEdge();

### PARALEL EDGES - kur kemi grafe nuk punon menyra e matrices,sepse per njeren mun me qit 1 per tjetren smun.
Kuzharazhu sahiri kerkon komponente me te forte sepse mos me pas pengesa te medha dhe defekte ne ate graf si psh per Directed cycle  .(Topoligical sort ose order).
(4 msime dhe 2 code exection) na vyn me dit ni graf dhe me dit me puno me to .(ushtrime).

### Minimum Spanning Trees
perdor undirected graph.
0.00 nuk hin ne MST.(Vlera 0 ).
Spanning Tree i G eshte nje nengraf T i cili :
eshte i lidhur 
aciklik.
perfshine te gjitha kulmet.
###Self-Loop pranohet ne MSP munet me pas por ne raste te rralla.
Ideja qe e perdorim MST eshte qe me gjet peshen me te vogel .
### Spanning Tree duhen me kon te lidhura (bolt lines) ndryshe nese so e lidht nuk o .
### Edge weighted Graph  quhet pasi qe e ka nje peshe unike (numer unik).
Per me ul nivelin qe me dy segmente me pas vleren e njejte duhet gjithmon me rujt double jo si int.(se mundesi me e madhe ne INT eshte qe me kon me peshe te njejte).
Shumes se peshave i thojme Cmim.
Sa me i ult cmimi qaq me efikas ose me i mire minimum spanning tree .
Pesha eshte shume e disa atributeve te ndryshme psh (distance ,kohe etj)

### Secili dizajne i secilit rrjet ne bote qe organizohet behet me MST.(Rruge,qarqe,hydraulic,komunikacion ) qe me i mrri ma shpejt edhe mas lehti qe me hargju ma 
pak .psh
kur kemi Face Recognition funksionon me MTS.
### Greedy MST Algorithm
Algoritmi me i thjeshte me gjet MST.
Per me gjet GMST duhet me bo prerje(CUT) sipas deshires  qe ne perfundim me gjet Minimalin pas qe ne fund duhet me gjet Minimum Spanning Tree ,
egzistojn disa brinje apo segmente qe e lidhin bashkesin I me II dhe quhen Crossing edge,me e vogla ka me qet pjese e MST.
Hapi fundit na mbet vetem ni kulm dhe nese ndodh mund ta vertetojm qe osht mire detyra.

### Kruskal Algorithm
Gjithmon e teston Spanning tree a ka loop-cycle.
Nuk eshte prej algoritmeve  me te mire sepse i fut te gjitha ne memorie dhe hargjon memorie per ato pa nevoj nganjeher dhe ka loop .
Nese ka loop e hek .

### Prim's  Algorithm
Primi starton prej 0 .
Psh nga 0 ne 7 tane vazhdon prej 7 shkon i gjet brinjet tjera bashk me 0 .
Logjiken e njejte si te Greedy .
Punon sikur me Heapsort.
Smun me ndodh loop.

### (Prim)Lazy Implementation 
Priority queue *
Ky perdor nodes(Kojshit e vet ) , nuk perdor bashkesi .
Nese ka loop i shton nmemorie sepse eshte lazy pasi qe nuk ia nin (i shti ne memorie edhe veq i le pa naj far lloj funksioni).
Loopat ia nisim e u hek prej memories kur vlerat e loopes duhet me i shti nMST.
### Prim eager implementation 
I kemi  disa array edgeTo[] dhe distTo[]
Kur e perdorim njonen vlere njeher mo nuk e perdorum se asnjeher nuk ka nje distanc me te shpejt se ajo .
Eager ka mundesi permisimi ateher kur mund te bejme diqka me shpejte .
Mun me bo cikel



### Shortes Path 
Nje graf mun te kete me shume se nje Topological sort .(Pytje provimit)
Perdoret per navigim edhe per rrjeta mas shumti .
Single source  prej nje kulmi i gjen rruget ma tshkurta .(ma i preferumi)
Single sink i viziton krejt kulmet dej sa ta gjeje ma tshkurtin.
Source sink Prej nje kulmi e gjen kulmin ma tshkurt tjeter.
All pairs i perdor krejt kulmet per me gjet ma tshkurtin  (perdoret per testim)
Krejt rruget me te shkurtra qe gjinden najkund quhen Edge Relaxation ,Procesi per me gjet rrug treja quhet Relaksiom i segmenteve .(si Edge relaxation),
kjo ndodh kur e qesim ni segment tri edhe kshyrum me zvoglu peshen e udhes.
3 algorime per Shortes path :
1. Dijakstra(no negative weight) me i miri dhe me i shpejti ,mun me pas pesha negative edhe pesha tnjejta nuk ka problem .
2.Acyclic(no cycle)
3.Bellman-Ford(no negativ cycles).-punon edhe me vlera negative edhe me pas cikle,por ka mangsi se nese nese ka cikel negativ nuk punon.

### Dijakstra
i permban dy array distTo[] dhe edgeTo[].
Kush e ka distancen me te vogel miret si source.

### Acyclic 
ne fillim e gjen Topological Order sepse nuk punon me cycle.(DFS)(distTo[],edgeTo[]).
Renditja shkon me Topological Order jo me peshen me te vogel .


### Bellman-Ford 
i provon prej tpares te krejt kulmet qe lidhet aj .
kalimet quhen me pass .
Nese ne pass e radhes nuk kemi update ather skena nevoj me shku me i bo pass tjerat se ska update.


### Ma i keqi algoritem per nga kompleksiteti eshte Bellman ford.
Dijakstra ma i miri (binaryheap).
Edhe topological sort eshte prej ma tmirve .


### Longest path  perdor topological order ,i marrum peshat ma tmdhaja .
Per me procesu paralel nevoitet Longest Path.

# Per Kolofium tdyt

### Stringet
Tri vetit themelore te stringave:
1.Length gjatesia e stringut 
2.Indexing vlera e stringut ne index.
3.Concatenation  bashkimi i dy stringjeve qe e bejne nje string me te gjate.
Stringjet kthehen ne substringje me ane te concatenation.
Algoritmet per sortim:
LSD-Ma e shpejta eshte per sortim ,kompleksitetin kohor e ka linear,
(eshte stabil sepse kur i ki dy karaktere te njejta nuk e kalojne kurr te parin ose te dytin ose te tretin dmth nuk e prishin sortin)
(inplace nuk eshte sepse i kemi dy array)
MSD-ma e ngadalte sepse ze shume vend me memorie,sepse nese kena me sortu shume na bjen me i da shume,gjate eksekutimin inner loop ka shume instruksione.



### Tries
Strukture qe do te perdoret per stringe  perdor key value ,eshte searching algorithm,eshte si symbol table,eshte collection i objekteve qe te gjitha objektet do te jene te tipit string.
Me tries do mundohemi te bejm searching stringe me metoden get(String key).
Algoritmi me i shpejte per me gjet stringe eshte ky (Tries).
Root eshte piknisja e tries ku e ka vleren null,tjerat kan value.
R-way -ka shume sasi te memories qe eshte e humbur,(njera prej te keqijav te tires).
Metoda per me shti elemente eshte put().
Dy lloje per search missing:
Nese mungon karakteri edhe nese ska index .Karakterin e lyp me CharAt().
###Ternary Search Tries 
Krejt karakterat ruhen ne nyje jo ne key
Secila nyje ka 3 femije me shume jo , me kusht qe me i vogli te shkoj majtas,i barabart ne mes dhe me te madh djathtas.
###TST VS Hashing 
TST punon veq me string ndersa Hashing punon me gjithqka.
Hashing duhet me i marr krejt vlerat e qelsave me i llogarit per me kshyr a ka collision ,ndersa nTST ska nevoj .
TST kontrollon aq karaktere sa i duhen ne qels,ndersa ne Hashin krejt qelsin e kontrollon.
Hashin nuk mundemi me perdor per sortim , TST mujm me perdor nifar lloji te sortimit,sa her ta prekum njerin prej karakterave qe bojm searching aj bohet sort.
TST eshte me e shpejt se hashin .
TST mun me pas search miss vetem te disa karaktera ndersa hashing searching hits edhe misses jon gati tnjejta.
(13 janar 2023 kolofiumi 2 )

### Substring Search

Dy length duhet me i kerku per me bo searching :Text dhe pattern(pattern eshte substringu qe e kerkojm)(Text eshte gjithmon me i madh se pattern).
Forensika kompjuterike - pjese qe lidhet me data security dhe me cyber security .
Screen Scraping - mundesh me nxjerr te dhena relevante prej faqeve .
Brute-force(Substring search algorithm) - I provon krejt kombinimet e mundshme dej sa te ket rezultat ,kerkimi behet karakter per karakter me metoden CharAt(),kompleksitetin e ka kuadratik N^2.
Mangesite:
Nuk mujm me garantu se kur kryet algoritmi (Linear-time).
Ne rastin me te keq eshte MN.
Back-up ne tekst,e bruteforce i run ne RAM e qaq shume run backup ne ram sa qe ka mundesi me u hargju rami.
Mismatch quajm kur nuk kemi lidhje te njejte .
i - i kerkon text
j - i kerkon pattern.
i+j=vlere qe ruhet ne buffer .
Knuth-Morris-Pratt Algorithm-eshte me i mire se Brute-force,implementohet per Virtual machine 
DFA simulation - perdoret per pergjime,e gjen veq ni fjal e pastaj nese qajo makin virtuale e gjen fjalen dmth bon match .(FBI).
Boyer-Moore - me i meqem se kta tjerte.skenon mbrapsht prej djath-majt,perparsi eshte se nese 
karakteri i fundit nuk eshte i sakt kta tjert hiq si kshyr.
Kur ka missmatch e kalon edhe shkon te karakteri tjeter.
Ne rastin me te keq eshte MN.
Rabin-Karp(fingerprint search)-ka logjiken me ndryshe,miret me hashing e paternave edhe ne baze te rezultatit te tyre ben match.
Kompleksitet kohore kane me te shpejte.
Perparsit:
1 search lehtesisht mund te zgjerohet per kerkim te patternave te shumefisht.
2 Perdor metoden e Hornerit deri ne 5 karakteret e pare,pastaj perdor metoden rolling hash.
Monte Carlo Versionin -jashtzakonisht shpesh eshte i sakt por jo gjithmon,kompleksitetin e ka linear.
Las Vegas  Gjithmon i sakt,shume shpesh ekzekutohet me kompleksitet kohore Lienar.
ne rastin me te keq eshte M N .
 



### Regular Expressions
Pattern Matching:
Regeksi na mundeson me i marr disa stringje te ndryshme edhe me ane te regular expressions i perfshin ato ne nje string.Kryen pune me shpejte se ato me lart.
Regeksi kur ta maroje maqinen na qon prej DFA ne NFA .
Regeksi na mundeson qe si DFA por gjen prej 1 e me shume substring.
Regeksi mundet me u perdor per validim ne web.(Email,URL,datat etj).
Regeksi mun prej nje substring me te dhon dy sene jo si te substring search qe veq 1 dhe vetem nje .
RFC-Request for Comments 


### Data Compression
Behet per 3 arsye :
Kursen hapsire memorike
Kursen kohe te transferit.
Ka shume me pak perseritje.
Gjate compresimit  ne menyre indirekte i enkriptojm ato te dhena.
Nevoitet per siguri tdhanave ,telekomunikacion ,algoritme.
Ligji i Moore-it Numri i tranzistoreve ne nje chip dyfishohet cdo 18-24 muje.
Ligji i Parkinson-it Te dhenat shtohen sa te ka hapsire .Foto,video,audio,text.
Modelet per compresim ndahen ne 3 lloje:
statike me e thjeshta dhe me primitive por shume e perdorshme.
dinamike model qe duhet me u lexu komplet imputi ,pastaj mas leximit gjehet frekuenca e perseritjes se karaktereve ne ate imput edhe gjenerohet kodi qe duhet me punu.
adaptiv kompresohen te dhenat ne ardhje e siper dmth sa mrrin ni bit i 1 tdhane aj meniher ia nis e kompreson edhe vazhdon nonstop(aplikohet zakonisht ne Livetime aplikacionet,Skype,etj).
Kodi i gjenomit permban 4 karaktere (ACTG).
Gjate kompresimit file nuk zvoglohet por zmadhohet.
Run-length codding eshte model statik 
Kompresimi i Huffman model dinamik ,punon me tries.
ne tablen e tij ka :char,freq,encoding.
Ky i shkrun prefix.(diqka qeshtu ke ,nese qet najsen se kush perdor prefix e prek Huffman).
Algoritmi LZW  model adabtiv.Perdor fjalor.

### Maximum Flow
Perdoret per rrjeta etj.
Ford-Fulkerson Algorithm- e percakton maksimumin e informatave qe mujn me rrjedh prej source ne target.
Ky problem Maximum flow ka natyre te dyfisht sepse nese nese e shohum nga njera ane ,algoritmi kshyr sasin ma te madhe te informatave me dergu prej source ntarget.
Ndersa ne anen tjeter algoritmi e kshyr Minimum Cut qysh me e zvoglu numrin sa ma shume qe me marr sa ma pak informata targeti prej source.
Zgjidhja eshte e njejte(Rezultati).
Nuk eshte i sigurt 100%.
Minimum Cut Logjiken e Greedy Algorithm dmth me prerje.
Kapaciteti eshte shuma e kapacitetit ne segment nga A ne B.
MaxFlow problemi
