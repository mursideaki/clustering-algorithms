# clustering-algorithms
# Kümeleme Algoritmalarının İncelenmesi: Wine Veri Seti

## Genel Bakış
Bu depo, Wine veri setini kullanarak kümeleme algoritmalarının ayrıntılı bir analizini sunar. Amaç, farklı kümeleme tekniklerini, değerlendirme metriklerini ve görselleştirme araçlarını tanıtmaktır.

### Dahil Edilen Algoritmalar:
1. **K-Means Kümeleme**
2. **Hiyerarşik Kümeleme**
3. **DBSCAN (Yoğunluk Temelli Kümeleme)**
4. **OPTICS (Ordering Points To Identify Clustering Structure)**
5. **HDBSCAN (Hierarchical Density-Based Spatial Clustering of Applications with Noise)**
6. **Gaussian Karışım Modelleri (GMM)**
7. **Spektral Kümeleme**
8. **Affinity Propagation**

### Boyut Azaltma Teknikleri:
- **PCA (Ana Bileşen Analizi)**: Doğrusal boyut azaltma için kullanılır.
- **t-SNE (t-dağıtılmış Stokastik Komşuluk Yerleştirme)**: Kümelemeleri düşük boyutlarda (genellikle 2D veya 3D) görünür hale getirir.
- **UMAP (Uniform Manifold Approximation and Projection)**: Veri setinin hem yerel hem de genel yapısını düşük boyutlarda yansıtır.

## Değerlendirme Ölçütleri
Kümeleme algoritmalarını değerlendirmek ve karşılaştırmak için aşağıdaki metrikler kullanılmıştır:

1. **Silhouette Skoru**: Bir noktanın kendi kümesine ve diğer kümelere olan benzerliğini ölçer.
2. **Davies-Bouldin Endeksi**: Küme kompaktlığını ve ayrışımını değerlendirir.
3. **Rand ve Ayarlanmış Rand İndeksi (ARI)**: Tahmin edilen ve gerçek küme atamaları arasındaki uyumu ölçer.
4. **V-Measure**: Homojenlik ve tamlık ölçülerini birleştirir.
5. **AIC (Akaike Bilgi Kriteri)** ve **BIC (Bayesyen Bilgi Kriteri)** (GMM için): Gaussian Karışım Modeli için optimal bileşen sayısını belirler.

## Görüselleştirme Araçları

1. **Boxplot**: Küme içindeki özellik dağılımlarını görüntüler.
2. **Dirsek Yöntemi (Elbow Plot)**: K-Means için optimal küme sayısını belirler.
3. **Dendrogram**: Hiyerarşik kümeleme sonuçlarını görüntüler.
4. **Reachability Plot**: OPTICS için küme yapısını gösterir.
5. **Isı Haritası (Heatmap)**: Özellikler arasındaki korelasyonu gösterir.
6. **Korelasyon Matrisi**: Veri seti özellikleri arasındaki ilişkileri gösterir.
7. **Pairplot**: Veri setindeki özellikler arasındaki çiftli ilişkileri görüntüler.


## Bu Depoyu Nasıl Kullanırsınız?
1. Depoyu klonlayın:
   ```bash
   git clone https://github.com/mursideaki/clustering-algorithms.git
   ```
2. Gerekli kütüphaneleri yükleyin:
   ```bash
   pip install -r requirements.txt
   ```
3. Jupyter Notebook dosyasını (**clustering.ipynb**) inceleyerek algoritmaların uygulanışını, görselleştirme tekniklerini ve sonuçları görüntüleyin.

## Önemli Bulgular
- **K-Means ve Hiyerarşik Kümeleme**, genel küme ayrımı için etkili oldu ancak küme sayısını dikkatlice ayarlamak gerekti.
- **DBSCAN ve HDBSCAN**, yoğunluk bazlı kümeleme yapısı için çok iyi performans gösterdi ve gürültüyü ayırt edebildi.
- **GMM**, daha karmaşık yapıları modellemek için esneklik sağladı en iyi sonuçları burada yakaladık ve AIC/BIC ile bileşen seçimini kolaylaştırdı.
- Boyut azaltma teknikleri olan **PCA**, **t-SNE** ve **UMAP**, yüksek boyutlu verilerin yorumlanabilirliğini arttırdı.

## Sonuç
Bu proje, farklı kümeleme tekniklerinin gücünü ve sınırlarını göstermekle birlikte, detaylı görselleştirme ve değerlendirme metrikleri sunarak kapsamlı bir kümeleme analizi sağlamaktadır.

## Gelecek Adımlar
- Bulguları genellemek için farklı veri setleriyle çalışılabilir.
- Derin öğrenme tabanlı kümeleme metotları projeye dahil edilebilir.

Herhangi bir öneriniz veya sorunuz varsa lütfen iletin!

