(Logistic Regression) ve denetimsiz öğrenme (k-Means) algoritmalarını karşılaştırdığımızda, denetimli öğrenme (Logistic Regression) çok daha iyi sonuçlar verir. Bunun nedeni, her iki öğrenme türünün veri üzerindeki çalışma biçimlerinden kaynaklanmaktadır.

1. Denetimli Öğrenme (Logistic Regression):
Neden daha iyi performans gösterir: Denetimli öğrenme, etiketlenmiş verilerle çalışır. Yani, model veri setinde hangi incelemelerin pozitif (1) ve hangilerinin negatif (0) olduğunu bilir. Bu nedenle, model verilerdeki örüntüleri tanıyıp, bu örüntülere göre tahmin yapar.
Performans Değerlendirmesi:
Doğruluk (Accuracy): Logistic Regression, genellikle %85-%90 doğruluk oranlarına ulaşır. Bu, modelin incelemeleri doğru sınıflandırma oranını gösterir.
Precision, Recall, F1 Score: Bu metrikler, sınıflandırma başarısının daha detaylı bir değerlendirmesini sağlar. Genellikle bu metriklerde de denetimli öğrenme modelleri iyi performans gösterir.
Logistic Regression gibi denetimli öğrenme modelleri, etiketli veri ile çalıştığından, belirli bir amaç için optimize edilebilir ve doğru sınıflandırmalar yapabilir.

2. Denetimsiz Öğrenme (k-Means):
Neden daha düşük performans gösterir: Denetimsiz öğrenme, veriler üzerinde hiçbir etiket bilgisine sahip değildir. Bu yüzden, yalnızca veri örüntülerine dayanarak kümeler oluşturur. k-Means modelinin iki küme (k=2) oluşturduğu bu durumda, model pozitif ve negatif yorumlar arasında net bir ayrım yapmadan verileri kümelemiştir.
Performans Değerlendirmesi:
Denetimsiz öğrenmede doğruluk veya precision/recall gibi metrikleri doğrudan kullanmak zor olabilir, çünkü modelin çıktıları belirli bir etikete sahip değildir. Ancak, verileri kümelere ayırarak doğal gruplar elde etmeye çalışır.
Kümeleme, özellikle sınıf dengesizlikleri olduğunda (pozitif ve negatif incelemeler dengesizse) yanlış kümelemelere yol açabilir. k-Means algoritması, incelemeleri iki kümeye ayırdı, ancak bu kümelerin gerçekten pozitif veya negatif incelemeler olup olmadığını kesin olarak bilemeyiz.
Denetimsiz öğrenme, sınıflandırma yerine daha çok veri içinde benzer gruplar bulmaya odaklanır. Ancak, etiketli bir problemde denetimsiz öğrenme modelleri genellikle daha düşük performans gösterir, çünkü modelin hangi verinin pozitif veya negatif olduğunu bilmemesi sınırlayıcıdır.

Sonuç:
Denetimli öğrenme (Logistic Regression) bu veri setinde daha iyi sonuçlar verir, çünkü model verilerin etiketlerini öğrenir ve bu etiketlere göre doğru tahminlerde bulunabilir.
Denetimsiz öğrenme (k-Means), veri setini kümelere ayırabilir ancak incelemeleri doğru bir şekilde sınıflandırma konusunda yetersiz kalır. Bu yüzden, sınıflandırma problemlerinde denetimli öğrenme yöntemleri tercih edilir.
