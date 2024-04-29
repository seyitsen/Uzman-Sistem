% Deri Hastalıkları Teşhisi Yapan Uzman Sistem

% ************************* EGZAMA HASTALIĞI*******************************

deri(egzama).

% KURALLAR

neden(egzama,yas).
neden(egzama,cinsiyet).
neden(egzama,stres).
neden(egzama,kotubeslenme).

nerede(egzama,'sac derisi').
nerede(egzama,yuz).
nerede(egzama,dirsekler).
nerede(egzama,el).

belirti(egzama,'kizariklik').
belirti(egzama,'kasinma').
belirti(egzama,'kepeklenme').
belirti(egzama,'deride renk degisikligi').
belirti(egzama,'cilt kurulugu').

egzamavarmi(egzama) :-
    belirti(egzama, 'kizariklik'),
    belirti(egzama, 'kasinma'),
    belirti(egzama, 'deride renk degisikligi'),
    nerede(egzama,'sac derisi');
    nerede(egzama,yuz);
    nerede(egzama,dirsekler);
    nerede(egzama,el).

sorgula_egzama(egzama) :-
    egzamavarmi(egzama),
    write('Egzama tespit edildi.').

/* Egzama Hastalığı Sorgu Ifadeleri
?-deri(X).
?-deri(egzama).
?-sorgula_egzama(egzama).
?-sorgula_egzama(sedef).
?-sorgula_egzama(X).
?-neden(egzama,X).
?-nerede(egzama,X).
?-belirti(egzama,X).
*/
    
% ************************* SEDEF HASTALIĞI*******************************

deri(sedef).

neden(sedef,stres).
neden(sedef,'cevresel faktorler').
neden(sedef,'genetik faktorler').
neden(sedef,'alkol ve sigara kullanimi').

nerede(sedef,el).
nerede(sedef,'sac derisi').
nerede(sedef,dirsek).
nerede(sedef,diz).

belirti(sedef,'deride pullanma').
belirti(sedef,'kırmızı veya beyazımsı lekeler').
belirti(sedef,'kuru ve catlamis cilt').
belirti(sedef,'deride kizariklik').
belirti(sedef,'deride agri').
belirti(sedef,'eklemlerde agri').

sedefvarmi(sedef) :-
    belirti(sedef,'deride pullanma'),
    belirti(sedef,'kırmızı veya beyazımsı lekeler'),
    belirti(sedef,'kuru ve catlamis cilt'),
    belirti(sedef,'deride kizariklik'),
    belirti(sedef,'deride agri'),
    belirti(sedef,'eklemlerde agri'),
    nerede(sedef,el);
    nerede(sedef,'sac derisi');
    nerede(sedef,dirsek);
    nerede(sedef,diz).

sorgula_sedef(sedef) :-
    sedefvarmi(sedef),
    write('sedef tespit edildi.').
    
/* Sedef Hastalığı Sorgu Ifadeleri
?-deri(X).
?-deri(sedef).
?-sorgula_sedef(sedef).
?-sorgula_sedef(egzama).
?-sorgula_sedef(X).
?-neden(sedef,X).
?-nerede(sedef,X).
?-belirti(sedef,X).
*/

% ************************* AKNE HASTALIĞI*******************************

deri(akne).

neden(akne,yas).
neden(akne,stres).
neden(akne,'sigara kullanimi').
neden(akne,'kozmetik urunler').

nerede(akne,'yuz').
nerede(akne,gogus).
nerede(akne,sirt).
nerede(akne,omuz).

belirti(akne,'siyah noktalar').
belirti(akne,'beyaz noktalar').
belirti(akne,'kasinma ve yanma').
belirti(akne,'noduller').
belirti(akne,'kistler').

aknevarmi(akne) :-
    belirti(akne,'siyah noktalar').
    belirti(akne,'beyaz noktalar').
    belirti(akne,'kasinma ve yanma').
    belirti(akne,'noduller').
    belirti(akne,'kistler'),
    nerede(akne,'yuz');
    nerede(akne,gogus);
    nerede(akne,sirt);
    nerede(akne,omuz).

sorgula_akne(akne) :-
    aknevarmi(akne),
    write('akne tespit edildi.').

/* Akne Hastalığı Sorgu Ifadeleri
?-deri(X).
?-deri(akne).
?-sorgula_akne(akne).
?-sorgula_akne(sedef).
?-sorgula_akne(X).
?-neden(akne,X).
?-nerede(akne,X).
?-belirti(akne,X).
*/
    
    
