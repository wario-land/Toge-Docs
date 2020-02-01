# Text

## In-game

### Text encoding

|        | x0 | x1 | x2 | x3 | x4 | x5 | x6 | x7 | x8 | x9 | xA | xB | xC | xD | xE | xF |
| ------ | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
| **0x** | 0  | 1  | 2  | 3  | 4  | 5  | 6  | 7  | 8  | 9  | A  | B  | C  | D  | E  | F  |
| **1x** | G  | H  | I  | J  | K  | L  | M  | N  | O  | P  | Q  | R  | S  | T  | U  | V  |
| **2x** | W  | X  | Y  | Z  | a  | b  | c  | d  | e  | f  | g  | h  | i  | j  | k  | l  |
| **3x** | m  | n  | o  | p  | q  | r  | s  | t  | u  | v  | w  | x  | y  | z  | .  | &  |
| **4x** | あ | い | う | え | お | か | き | く | け | こ | さ | し | す | せ | そ | た |
| **5x** | ち | つ | て | と | な | に | ぬ | ね | の | は | ひ | ふ | へ | ほ | ま | み |
| **6x** | む | め | も | や | ゆ | よ | ら | り | る | れ | ろ | わ | を | ん | ぁ | ぃ |
| **7x** | ぅ | ぇ | ぉ | ゃ | ゅ | ょ | っ | が | ぎ | ぐ | げ | ご | ざ | じ | ず | ぜ |
| **8x** | ぞ | だ | ぢ | づ | で | ど | ば | び | ぶ | べ | ぼ | ぱ | ぴ | ぷ | ぺ | ぽ |
| **9x** | ア | イ | ウ | エ | オ | カ | キ | ク | ケ | コ | サ | シ | ス | セ | ソ | タ |
| **Ax** | チ | ツ | テ | ト | ナ | ニ | ヌ | ネ | ノ | ハ | ヒ | フ | ヘ | ホ | マ | ミ |
| **Bx** | ム | メ | モ | ヤ | ユ | ヨ | ラ | リ | ル | レ | ロ | ワ | ヲ | ン | ァ | ィ |
| **Cx** | ゥ | ェ | ォ | ャ | ュ | ョ | ッ | ガ | ギ | グ | ゲ | ゴ | ザ | ジ | ズ | ゼ |
| **Dx** | ゾ | ダ | ヂ | ヅ | デ | ド | バ | ビ | ブ | ベ | ボ | パ | ピ | プ | ペ | ポ |
| **Ex** | ヴ | '  | ,  | .  | ー  | ~  | …  | !  | ?  | (  | )  | 「 | 」 | 『 | 』 | [  |
| **Fx** | ]  | ℃ | -  |    |    |    |    |    |    |    |    |    |    |    |    |    |

### Pointer tables

| Offset     | Count  | Description
| ---------- | ------ | -----------
| 0x0863956C | 0x07   | Japanese passage names
| 0x08639588 | 0x07   | English passage names
| 0x0863A31C | 0x0F   | Japanese stage names
| 0x0863A3AC | 0x0F   | English stage names
| 0x0863D8A0 | 0x10   | Japanese CD titles
| 0x0863D8E0 | 0x10   | English CD titles
| 0x0863D920 | 0x0A   | Japanese karaoke lyrics
| 0x0863D948 | 0x0D   | English karaoke lyrics
| 0x086E32C4 | 0x0C   | Japanese mini-game texts
| 0x086E32F4 | 0x0C   | English mini-game texts
| 0x08730114 | 0x0F   | Japanese Item Shop texts
| 0x08730150 | 0x0F   | English Item Shop texts

### Passage names

The strings are 26 character long, left and right padded with 0xFF to be centered.

| Index | Offset     | Language | Value
| ----- | ---------- | -------- | -----
| 0x00  | 0x0864C758 | JP       | さいしょのつうろ
| 0x01  | 0x0864C772 | EN       | Entry Passage
| 0x02  | 0x0864C78C | JP       | みどりのつうろ
| 0x03  | 0x0864C7A6 | EN       | Emerald Passage
| 0x04  | 0x0864C7C0 | JP       | あかのつうろ
| 0x05  | 0x0864C7DA | EN       | Ruby Passage
| 0x06  | 0x0864C7F4 | JP       | きいろのつうろ
| 0x07  | 0x0864C80E | EN       | Topaz Passage
| 0x08  | 0x0864C828 | JP       | あおのつうろ
| 0x09  | 0x0864C842 | EN       | Sapphire Passage
| 0x0A  | 0x0864C85C | JP       | おうごんのピラミッド
| 0x0B  | 0x0864C876 | EN       | Golden Pyramid
| 0x0C  | 0x0864C890 | JP       | サウンドルーム
| 0x0D  | 0x0864C8AA | EN       | Sound Room

### Stage names

| Index | Offset     | Language | Value
| ----- | ---------- | -------- | -----
| 0x00  | 0x0865CEC4 | JP       | はじまりのいせき
| 0x01  | 0x0865CEDE | EN       | Hall of Hieroglyphs
| 0x02  | 0x0865CEF8 | JP       | さいしょのボス ピンキー
| 0x03  | 0x0865CF12 | EN       | Spoiled Rotten
| 0x04  | 0x0865CF2C | JP       | ミニゲームやさん
| 0x05  | 0x0865CF46 | EN       | Mini-Game Shop
| 0x06  | 0x0865CF60 | JP       | ヤシのきじま
| 0x07  | 0x0865CF7A | EN       | Palm Tree Paradise
| 0x08  | 0x0865CF94 | JP       | おはなばたけ
| 0x09  | 0x0865CFAE | EN       | Wildflower Fields
| 0x0A  | 0x0865CFC8 | JP       | なぞのちていこ
| 0x0B  | 0x0865CFE2 | EN       | Mystic Lake
| 0x0C  | 0x0865CFFC | JP       | あめのジャングル
| 0x0D  | 0x0865D016 | EN       | Monsoon Jungle
| 0x0E  | 0x0865D030 | JP       | みどりのボス フラワナ
| 0x0F  | 0x0865D04A | EN       | Cractus
| 0x10  | 0x0865D064 | JP       | ミニゲームやさん
| 0x11  | 0x0865D07E | EN       | Mini-Game Shop
| 0x12  | 0x0865D098 | JP       | あやしいこうじょう
| 0x13  | 0x0865D0B2 | EN       | The Curious Factory
| 0x14  | 0x0865D0CC | JP       | ひみつのはいきぶつしょりじょう
| 0x15  | 0x0865D0E6 | EN       | The Toxic Landfill
| 0x16  | 0x0865D100 | JP       | -40℃のれいぞうこ
| 0x17  | 0x0865D11A | EN       | 40 Below Fridge
| 0x18  | 0x0865D134 | JP       | ピンボールタワー
| 0x19  | 0x0865D14E | EN       | Pinball Zone
| 0x1A  | 0x0865D168 | JP       | あかのボス コンダラー
| 0x1B  | 0x0865D182 | EN       | Cuckoo Condor
| 0x1C  | 0x0865D19C | JP       | ミニゲームやさん
| 0x1D  | 0x0865D1B6 | EN       | Mini-Game Shop
| 0x1E  | 0x0865D1D0 | JP       | つみきのおしろ
| 0x1F  | 0x0865D1EA | EN       | Toy Block Tower
| 0x20  | 0x0865D204 | JP       | すごろくのくに
| 0x21  | 0x0865D21E | EN       | The Big Board
| 0x22  | 0x0865D238 | JP       | らくがきのもり
| 0x23  | 0x0865D252 | EN       | Doodle Woods
| 0x24  | 0x0865D26C | JP       | ドミノストリート
| 0x25  | 0x0865D286 | EN       | Domino Row
| 0x26  | 0x0865D2A0 | JP       | きいろのボス シッキー
| 0x27  | 0x0865D2BA | EN       | Aerodent
| 0x28  | 0x0865D2D4 | JP       | ミニゲームやさん
| 0x29  | 0x0865D2EE | EN       | Mini-Game Shop
| 0x2A  | 0x0865D308 | JP       | みかづきのゴーストタウン
| 0x2B  | 0x0865D322 | EN       | Crescent Moon Village
| 0x2C  | 0x0865D33C | JP       | アラビアンナイト
| 0x2D  | 0x0865D356 | EN       | Arabian Night
| 0x2E  | 0x0865D370 | JP       | ほのおのどうくつ
| 0x2F  | 0x0865D38A | EN       | Fiery Cavern
| 0x30  | 0x0865D3A4 | JP       | ホラーマンション
| 0x31  | 0x0865D3BE | EN       | Hotel Horror
| 0x32  | 0x0865D3D8 | JP       | あおのボス キャバット
| 0x33  | 0x0865D3F2 | EN       | Catbat
| 0x34  | 0x0865D40C | JP       | ミニゲームやさん
| 0x35  | 0x0865D426 | EN       | Mini-Game Shop
| 0x36  | 0x0865D440 | JP       | さいごのつうろ
| 0x37  | 0x0865D45A | EN       | Golden Passage
| 0x38  | 0x0865D474 | JP       | ピラミッドのぬし ヨーキ
| 0x39  | 0x0865D48E | EN       | Golden Diva
| 0x3A  | 0x0865D4A8 | JP       | ミニゲームやさん
| 0x3B  | 0x0865D4C2 | EN       | Mini-Game Shop

### CD titles

| Index | Offset     | Language | Value
| ----- | ---------- | -------- | -----
| 0x00  | 0x086CB488 | JP       | あの ひつじかい に ついて しってる 2,3のこと
| 0x01  | 0x086CB4A2 | EN       | About That Shepherd
| 0x02  | 0x086CB4BC | JP       | その つぎに かわらない モノ
| 0x03  | 0x086CB4D6 | EN       | Things That Never Change
| 0x04  | 0x086CB4F0 | JP       | あした の けつあつ
| 0x05  | 0x086CB50A | EN       | Tomorrow's Blood Pressure
| 0x06  | 0x086CB524 | JP       | たちくらみ の むこうがわ
| 0x07  | 0x086CB53E | EN       | Beyond the Headrush
| 0x08  | 0x086CB558 | JP       | りゅうぼく と アイルランドいぬ
| 0x09  | 0x086CB572 | EN       | Driftwood & the Island Dog
| 0x0A  | 0x086CB58C | JP       | さいばんかん の あし
| 0x0B  | 0x086CB5A6 | EN       | The Judge's Feet
| 0x0C  | 0x086CB5C0 | JP       | つき の でんちゅう
| 0x0D  | 0x086CB5DA | EN       | The Moon's Lamppost
| 0x0E  | 0x086CB5F4 | JP       | ヤワラカイ こうら
| 0x0F  | 0x086CB60E | EN       | Soft Shell
| 0x10  | 0x086CB628 | JP       | やっぱり ねむいね……
| 0x11  | 0x086CB642 | EN       | So Sleepy
| 0x12  | 0x086CB65C | JP       | みぢかい ふとん
| 0x13  | 0x086CB676 | EN       | The Short Futon
| 0x14  | 0x086CB690 | JP       | アボカド ソング
| 0x15  | 0x086CB6AA | EN       | Avocado Song
| 0x16  | 0x086CB6C4 | JP       | ハエおとこ
| 0x17  | 0x086CB6DE | EN       | Mr. Fly
| 0x18  | 0x086CB6F8 | JP       | きのう の コトバ
| 0x19  | 0x086CB712 | EN       | Yesterday's Words
| 0x1A  | 0x086CB72C | JP       | おつかい
| 0x1B  | 0x086CB746 | EN       | The Errand
| 0x1C  | 0x086CB760 | JP       | きみ と クツ
| 0x1D  | 0x086CB77A | EN       | You and Your Shoes
| 0x1E  | 0x086CB794 | JP       | エーテルおじさん と プラナリア
| 0x1F  | 0x086CB7AE | EN       | Mr. Ether & Planaria

### Karaoke

The titles are centered, the lyrics are aligned to the left.

| Index | Offset     | Language | Value
| ----- | ---------- | -------- | -----
| 0x00  | 0x086D3108 | JP       | Sunny Side up
| 0x01  | 0x086D3122 | JP       | ウクレレ みたいな たびを しよー
| 0x02  | 0x086D313C | JP       | あるいて いこう つきの かけらを ひろいながら
| 0x03  | 0x086D3156 | JP       | ちずの かわりに キャンバス
| 0x04  | 0x086D3170 | JP       | にじの しずくで (そめましょう)
| 0x05  | 0x086D318A | JP       | ひのでに まにあうように
| 0x06  | 0x086D31A4 | JP       | ぼやけた とけいは おいていこう
| 0x07  | 0x086D31BE | JP       | うみに タメいき とかしーて
| 0x08  | 0x086D31D8 | JP       | いしに こえを きざもーぉ
| 0x09  | 0x086D31F2 | JP       | つきを スープに うかべたら
| 0x0A  | 0x086D320C | JP       | ヒョウがらの くもが わらう
| 0x0B  | 0x086D3226 | EN       | MEDAMAYAKI
| 0x0C  | 0x086D3240 | EN       | UKURERE MITAINA
| 0x0D  | 0x086D325A | EN       | TABIWO SHIYO
| 0x0E  | 0x086D3274 | EN       | ARUITE IKO TSUKINO
| 0x0F  | 0x086D328E | EN       | KAKERAWO HIROINAGARA
| 0x10  | 0x086D32A8 | EN       | CHIZUNO KAWARINI KYANBASU
| 0x11  | 0x086D32C2 | EN       | NIJINO SHIZUKUDE
| 0x12  | 0x086D32DC | EN       | (SOMEMASHO)
| 0x13  | 0x086D32F6 | EN       | HINODENI MANIAUYONI
| 0x14  | 0x086D3310 | EN       | BOYAKETA TOKEIWA OITEKO
| 0x15  | 0x086D332A | EN       | UMINI TAMEIKI TOKASHITE
| 0x16  | 0x086D3344 | EN       | ISHINI KOEWO KIZAMO
| 0x17  | 0x086D335E | EN       | TSUKIWO SUPUNI UKABETARA
| 0x18  | 0x086D3378 | EN       | HYOUGARANO KUMOGA WARAU

### Mini-games

The strings are aligned to the left.

| Index | Offset     | Language | Value
| ----- | ---------- | -------- | -----
| 0x00  | 0x086F481C | JP       | ミニゲームデ メダルヲ ゲット シマショウ!    
| 0x01  | 0x086F4836 | EN       | Win medals in mini-games. 
| 0x02  | 0x086F4850 | JP       | スポーツバンノウナ アナタハ 『ワリオ ホームラン』
| 0x03  | 0x086F486A | EN       | Wario's Homerun Derby     
| 0x04  | 0x086F4884 | JP       | オンガクズキナ アナタハ 『ワリオ ホッパー』   
| 0x05  | 0x086F489E | EN       | The Wario Hop             
| 0x06  | 0x086F48B8 | JP       | キオクリョクノヨイ アナタハ 『ワリオ ルーレット』
| 0x07  | 0x086F48D2 | EN       | Wario's Roulette          
| 0x08  | 0x086F48EC | JP       | コインガ タリナイノデ ゲームハ デキマセン.   
| 0x09  | 0x086F4906 | EN       | You need more coins.      
| 0x0A  | 0x086F4920 | JP       | タダイマ セイサクチュウ.             
| 0x0B  | 0x086F493A | EN       | Under construction.       
| 0x0C  | 0x086F4954 | JP       | モウチョット ミニゲーム シマセンカ?       
| 0x0D  | 0x086F496E | EN       | Want to play some more?   
| 0x0E  | 0x086F4988 | JP       | コインヲカセイデ マタ キテクダサイネ.      
| 0x0F  | 0x086F49A2 | EN       | Come back after saving up.
| 0x10  | 0x086F49BC | JP       | イッテラッシャイ!                 
| 0x11  | 0x086F49D6 | EN       | Come again.               
| 0x12  | 0x086F49F0 | JP       | オカエリ ナサイマシ.               
| 0x13  | 0x086F4A0A | EN       | Welcome back!             
| 0x14  | 0x086F4A24 | JP       | ハイスコア コウシン オメデトウゴザイマス.    
| 0x15  | 0x086F4A3E | EN       | You got a new high score! 
| 0x16  | 0x086F4A58 | JP       | イッカイクライ アソンデ イキマショウヨ.     
| 0x17  | 0x086F4A72 | EN       | Don't you want to play? 

### Item Shop

| Index | Offset     | Language | Value
| ----- | ---------- | -------- | -----
| 0x00  | 0x0873D458 | JP       | なにもかわずに でていくのネ.そうなのネ?     
| 0x01  | 0x0873D472 | EN       | Leaving without buying?   
| 0x02  | 0x0873D48C | JP       | りんごのカタチの ばくだんヨ.たべちゃダメ.    
| 0x03  | 0x0873D4A6 | EN       | That's an Apple Bomb.     
| 0x04  | 0x0873D4C0 | JP       | ドカーンな たいほうなのヨ.でも ちいさいのヨ.  
| 0x05  | 0x0873D4DA | EN       | That's a Blast Cannon.    
| 0x06  | 0x0873D4F4 | JP       | しろマンヨ.しろいから しろマンなのヨ.      
| 0x07  | 0x0873D50E | EN       | That's Vizorman.          
| 0x08  | 0x0873D528 | JP       | ラッパなのヨ.ヨワそうだけど ヨワくないヨ.    
| 0x09  | 0x0873D542 | EN       | That's a Bugle.           
| 0x0A  | 0x0873D55C | JP       | クロいイヌヨ.メがコワいなんて いわないのヨ.   
| 0x0B  | 0x0873D576 | EN       | That's a Black Dog.       
| 0x0C  | 0x0873D590 | JP       | おっきい クチびるヨ.テキに ブッチュしちゃうのヨ.
| 0x0D  | 0x0873D5AA | EN       | Those are the Large Lips. 
| 0x0E  | 0x0873D5C4 | JP       | おやじの げんこつヨ.じつは えどっコなのヨ.   
| 0x0F  | 0x0873D5DE | EN       | That's a Big Fist.        
| 0x10  | 0x0873D5F8 | JP       | クロいドラゴンヨ.イヌに にてるけど ちがうヨ.  
| 0x11  | 0x0873D612 | EN       | That's a Black Dragon.    
| 0x12  | 0x0873D62C | JP       | ステキな えがおを アナタに プレゼント!     
| 0x13  | 0x0873D646 | EN       | Here's a smile for you!   
| 0x14  | 0x0873D660 | JP       | アイテムショップに ようこそなのヨ.        
| 0x15  | 0x0873D67A | EN       | Welcome to the Item Shop. 
| 0x16  | 0x0873D694 | JP       | メダル たりないのヨ.うらないヨ.         
| 0x17  | 0x0873D6AE | EN       | You need more medals.     
| 0x18  | 0x0873D6C8 | JP       | おかいあげ ありがとなのヨ.            
| 0x19  | 0x0873D6E2 | EN       | Thank you!                
| 0x1A  | 0x0873D6FC | JP       | ミニゲームで メダル てにいれてくるのヨ.     
| 0x1B  | 0x0873D716 | EN       | Go play some mini-games.  
| 0x1C  | 0x0873D730 | JP       | ウふっ!                      
| 0x1D  | 0x0873D74A | EN       | Hmph! 

## Credits

### Text encoding

#### One-tile high

|        | x0 | x1 | x2 | x3 | x4 | x5 | x6 | x7 | x8 | x9 | xA | xB | xC | xD | xE | xF |
| ------ | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
| **4x** | A  | B  | C  | D  | E  | F  | G  | H  | I  | J  | K  | L  | M  | N  | O  | P  |
| **5x** | Q  | R  | S  | T  | U  | V  | W  | X  | Y  | Z  | .  | ,  |    |    |    |    |

#### Two-tile high, upper half

|        | x0 | x1 | x2 | x3 | x4 | x5 | x6 | x7 | x8 | x9 | xA | xB | xC | xD | xE | xF |
| ------ | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
| **6x** | A  | B  | C  | D  | E  | F  | G  | H  | I  | J  | K  | L  | M  | N  | O  | P  |
| **7x** | Q  | R  | S  | T  | U  | V  | W  | X  | Y  | Z  |    |    |    |    |    |    |
| **Ax** | a  | b  | c  | d  | e  | f  | g  | h  | i  | j  | k  | l  | m  | n  | o  | p  |
| **Bx** | q  | r  | s  | t  | u  | v  | w  | x  | y  |    |    |    |    |    |    |    |

#### Two-tile high, lower half

|        | x0 | x1 | x2 | x3 | x4 | x5 | x6 | x7 | x8 | x9 | xA | xB | xC | xD | xE | xF |
| ------ | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
| **8x** | A  | B  | C  | D  | E  | F  | G  | H  | I  | J  | K  | L  | M  | N  | O  | P  |
| **9x** | Q  | R  | S  | T  | U  | V  | W  | X  | Y  | Z  |    |    |    |    |    |    |
| **Cx** | a  | b  | c  | d  | e  | f  | g  | h  | i  | j  | k  | l  | m  | n  | o  | p  |
| **Dx** | q  | r  | s  | t  | u  | v  | w  | x  | y  | .  |    |    |    |    |    |    |

### Textmaps

| Offset     | Count  | Description
| ---------- | ------ | -----------
| 0x08747108 | 0x0E   | Textmap pointers

| Index | Offset     | Value
| ----- | ---------- | -----
| 0x00  | 0x08789FCC | Executive Producer
| 0x01  | 0x0878A4CC | Producer
| 0x02  | 0x0878A9CC | Director, Supervisor
| 0x03  | 0x0878AECC | Programmers
| 0x04  | 0x0878B3CC | Designers
| 0x05  | 0x0878B8CC | Designers
| 0x06  | 0x0878BDCC | Music
| 0x07  | 0x0878C2CC | Voice
| 0x08  | 0x0878C7CC | Artwork
| 0x09  | 0x0878CCCC | Special Thanks 
| 0x0A  | 0x0878D1CC | Super Mario Club 
| 0x0B  | 0x0878D6CC | Super Mario Club 
| 0x0C  | 0x0878DBCC | Super Mario Club 
| 0x0D  | 0x0878E0CC | Copyright Notice

* Textmap size: 1280 bytes
* Textmap width: 32 tiles
* Textmap height: 20 tiles
* Tile size: 2 bytes

### Notes

* The Copyright notice textmap seems to be unused. 
* There's a weird tile in the Music textmap.
