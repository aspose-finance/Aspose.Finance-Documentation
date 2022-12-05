---
title: XBRL ve iXBRL dosyalarını Python'de doğrulayın
linktitle: XBRL ve iXBRL dosyalarını doğrulayın
keywords: xbrl taxonomy,xbrl,ixbrl,xbrl linkbases,xbrl Instances
description: Python Finance Kütüphane API, XBRL ve iXBRL dosyalarını doğrulayabilir. Daha fazla bilgi için lütfen bu makalede verilen örnek kodlara bakın.
type: docs
weight: 30
url: /tr/python-net/validate-xbrl-and-ixbrl-files/
---
## **XBRL örnek dosyasını Python'de doğrulayın**
 XBRL Bulut Sunucuları, XBRL Bağlantı Tabanları ve XBRL Taksonomi Şemaları, belirtilen sözdizimi gereksinimlerine UYMALIDIR[XBRL spesifikasyonu](http://www.xbrl.org/Specification/XBRL-2.1/REC-2003-12-31/XBRL-2.1-REC-2003-12-31+corrected-errata-2013-02-20.html). Bunları doğrulamak için XbrlInstance sınıfı, valid() yöntemini sağlar.

Aşağıdaki Python kod parçacığı, bir XBRL örnek belgesinin nasıl doğrulanacağını gösterir.

{{< gist "aspose-finance-gists" "e1df624c58dc6f522a87f29ceb041dd9" "validate-xbrl-instance-file.py" >}}
## **iXBRL dosyasını Python'de doğrula**
 bu[iXBRL spesifikasyonu](http://www.xbrl.org/specification/inlinexbrl-part1/rec-2013-11-18/inlinexbrl-part1-rec-2013-11-18.html) birçok doğrulama kuralı tanımlar. iXBRL dosyalarını doğrulamak için InlineXbrlDocument sınıfı bir valid() yöntemi sağlar.

Aşağıdaki Python kod parçacığı, bir iXBRL örnek belgesinin doğrulanmasını gösterir.

{{< gist "aspose-finance-gists" "e1df624c58dc6f522a87f29ceb041dd9" "validate-ixbrl-file.py" >}}
## **Doğrulama hata kodları**
 ValidationErrorCode numaralandırmasında, her doğrulama kuralı için doğrulama hata kodları tanımlanır.
Hata kodu tanımları aşağıdadır:

- BAĞLAM_DÖNEM_NUMARA_BAŞLAT_ZAMAN: Bağlam dönemi türü süre, ancak başlangıç tarihi yok.
- BAĞLAM_DÖNEM_NUMARA_SON_ZAMAN: Bağlam dönemi türü süre, ancak bitiş tarihi yok.
- BAĞLAM_DÖNEM_BAŞLAT_SONRASINDA_END: Bağlam dönemi türü süre, ancak bitiş tarihi başlangıç tarihinden önce.
- BAĞLAM_ANİ_NO_TIME: Bağlam dönemi türü anlıktır, ancak anlık tarihi yoktur.
- BAĞLAM_SENARYO_XBRL_NAMESPACE: Bağlam senaryosunda XBRL ad alanı düğümü olamaz.
- BAĞLAM_SENARYO_XBRL_İKAME_GRUP: Bağlam senaryosu, XBRL ad alanında tanımlanan öğeler için ikame grubunda bir öğeye sahip olamaz.
- BAĞLAM_SENARYO_BOŞ: Bağlam senaryosu boş olamaz.
- BAĞLAM_BÖLÜM_XBRL_NAMESPACE: Bağlam segmenti, XBRL ad alanı düğümüne sahip olamaz.
- BAĞLAM_BÖLÜM_XBRL_SUBSTITUTIONGROUP: Bağlam segmenti, XBRL ad alanında tanımlanan öğeler için ikame grubunda öğeye sahip olamaz.
- BAĞLAM_BÖLÜM_BOŞ: Bağlam segmenti boş olamaz.
- ÖĞE_NUMARA_BAĞLAM: Öğenin bir bağlamı olmalıdır.
- ÖĞE_DÖNEM_TİP_FİKİR AYRILIĞI_WITH_CONTEXT: Öğe, bağlamla dönem türü çakışmasına sahip.
- ÖĞE_SAYISAL_NO_UNIT: Öğe sayısaldır ve bir birimi olmalıdır.
- PARASAL_ÖĞE_NUMARA_BEKAR_UNIT_MEASURE: Öğe parasal bir türdür ve tek bir ölçü birimine sahip olmalıdır.
- PARASAL_ÖĞE_NO_ISO4217: Öğe, parasal bir türdür ve Iso 4217 stil birim ölçüsüne sahip olmalıdır.
- PAYLAŞ_ÖĞE_NUMARA_BEKAR_UNIT_MEASURE: Öğe bir paylaşım türüdür ve tek bir birim ölçüsü olmalıdır.
- PAYLAŞ_ÖĞE_NUMARA_PAYLAŞ_UNIT_MEASURE: Öğe, paylaşım türüdür ve bir xbrli:shares birim ölçüsüne sahip olmalıdır.
- SIFIR_ÖĞE_İLE BİRLİKTE_KESİNLİK_OR_DECIMALS: Öğe sıfırdır ve kesinliği veya ondalık sayıları olmamalıdır.
- KESİR_ÖĞE_İLE BİRLİKTE_KESİNLİK_OR_DECIMALS: Öğe bir kesir türüdür ve kesinliği veya ondalık sayıları olmamalıdır.
- SAYISAL_ÖĞE_İLE BİRLİKTE_İKİSİ BİRDEN_KESİNLİK_VE_ONDALIKLAR: Öğe sayısal bir türdür ve hem kesinlik hem de ondalık sayılar içermemelidir.
- SAYISAL_ÖĞE_OLMADAN_KESİNLİK_OR_DECIMALS: Öğe sayısal bir türdür ve kesinliği veya ondalık sayıları olmalıdır.
- OLMAYAN_SAYISAL_ÖĞE_İLE BİRLİKTE_KESİNLİK_VEYA_ONDALIKLAR: Öğe sayısal bir tür değildir ve kesinlik veya ondalık sayılar içermemelidir.
- DİPNOT_ark_İTİBAREN_OLUMSUZLUK_BULUNDU: Loc'tan Dipnot yayı bulunamadı.
- DİPNOT_ark_İLE_OLUMSUZLUK_BULUNDU: Dipnottan Dipnota geçiş bulunamıyor.
- TANIM_ark_İTİBAREN_OLUMSUZLUK_BULUNDU: Loc'tan Tanım yayı bulunamadı.
- TANIM_ark_İLE_OLUMSUZLUK_BULUNACAK: Loc için Tanım arkı bulunamadı.
- ÖZ_Takma ad_TANIM_ark_DIFFERENT_TYPE: Essence-alias Tanım arkın farklı türleri vardır.
- ÖZ_Takma ad_TANIM_ark_FARKLI_DÖNEM_TİP: Essence-alias Tanım arc'ın farklı periodType'ları vardır.
- ÖZ_Takma ad_TANIM_ark_DIFFERENT_BALANCE: Essence-alias Tanım arkın farklı dengeleri vardır.
- HESAPLAMA_ark_İTİBAREN_OLUMSUZLUK_BULUNDU: Loc'tan Hesaplama yayı bulunamadı.
- HESAPLAMA_ark_İLE_OLUMSUZLUK_BULUNDU: Loc için Hesaplama yayı bulunamadı.
- ETİKET_ark_İTİBAREN_OLUMSUZLUK_BULUNDU: Loc'tan Lable yayı bulunamadı.
- ETİKET_ark_İLE_OLUMSUZLUK_BULUNDU: Loc'a etiket yayı bulunamadı.
- SUNUM_ark_İTİBAREN_OLUMSUZLUK_BULUNDU: Loc'tan bir Sunum yayı bulunamadı.
- SUNUM_ark_İLE_OLUMSUZLUK_BULUNDU: Loc için bir Sunum yayı bulunamadı.
- REFERANS_ark_İTİBAREN_OLUMSUZLUK_BULUNDU: Loc'tan bir Referans yayı bulunamadı.
- REFERANS_ark_İLE_OLUMSUZLUK_BULUNDU: Loc'a bir Referans yayı bulunamadı.
### **Standart doğrulama hata mesajı örneği**
![yapılacaklar:resim_alternatif_Metin](validate-xbrl-and-ixbrl-files_1.png)

Yukarıdaki bir XBRL örneğidir, “cd1” bağlamını tanımlar, bu bağlam periyodu türü süre, başlangıç tarihi 2002-03-31, bitiş tarihi 2001-03-31, yani bitiş tarihi başlangıç tarihinden önce. XBRL spesifikasyonu, bölüm 4.7.2'de doğrulama kuralını tanımlar: "bitişTarihi, ilgili başlangıçTarihi'nin belirtilen veya ima edilen zamanından daha sonra olan bir zaman noktasını belirtmeli veya ima etmelidir". Bu kurala göre, bu XBRL örneği geçerli değil.
## **XBRL'i doğrulayın ve standart hata mesajı alın**
Aşağıdaki kod, XBRL örneğini doğrular ve standart hata mesajını verir.

{{< gist "aspose-finance-gists" "e1df624c58dc6f522a87f29ceb041dd9" "ValidateXBRLWithStardardErrorMessage.py" >}}

Aşağıdaki görüntü çıktıyı gösterir:

![yapılacaklar:resim_alternatif_Metin](validate-xbrl-and-ixbrl-files_2.png)



