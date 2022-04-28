# Araştırma Ödevleri:

- [Araştırma Projesi 1 - Lateinit](#1)
- [Araştırma Projesi 2 - Tools Namespace](#2)


### <a name="1"></a> Araştırma Projesi 1

- Lateinit neden kullanıyoruz?
- Lateinit kullanımından bahseder misiniz?
- Lateinit için bir örnek kullanım gösterir misiniz ?
      
      Cevap:
     Lateinit, türkçe olarak düşündüğümüzde geç başlatmak anlamına gelmektedir. Lateinit, değişkenin kullanılmadan önce başlatılacağına emin olduğumuz zamanlarda            kullanılmaktadır. Bir lateinit değikenini kullanmadan önce başlatmazsak “lateinit property has not been initialized” hatasını alırız. Lateinit sadece var olan          değişkenlerde kullanılmaktadır. Aynı zamanda lateinit kelimesi değişkenler daha sonraki durumlarda değişirse yani kullandığımız değişkenler değişken ise lateinit      kullanabiliriz. Ancak lateinit kullanırken değişken null türde olamaz ve long, int gibi ilkel olmayan veri türleri iin kullanılmaz.
     
     
     private lateinit var button: Button
    private lateinit var dice :ImageView

    constructor(parcel: Parcel) : this() {

    }

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)
        button=findViewById(R.id.mybutton)
        dice=findViewById(R.id.dice)
        button.setOnClickListener (this)


        }



### <a name="2"></a> Araştırma Projesi 2


- Layout dizini içinde xml dosyalarımız için kullandığımız namespace nedir ?
- Neden kullanılmaktadır ?
- Nasıl kullanılmalıdır ?
- Bir adet Tools (tools namespace) attribute kullanımını gösterir misiniz ? 
       Cevap:
       
       Bir uygulama geliştirirken layout dizini içinde kullandıpımız xml dosyasını tool attribute(tools namespace) ile mümkündür. 
       Tasarım tarafında yapılan değişkenlerin çıktısını uygulamayı çalıştırmadan direk görebilmemizi sağlamaktadır. 
       Tasarım özelliklerini veya derleme zaman davranışlarını etkinleştiren XML özelliklerini destekler.
       Kullanabilmemiz için activity_main.xml dosyamız içinde "xmlns:tools="http://schemas.android.com/tools"" tanımlamamız gerekmektedir.
       Örnek vermek gerekirse:
       -Tools namespace kullanmadan
       android:text="Get unlimited"
       -Tools kullanarak
       tools:text="Get unlimited"
       
       ## <a name="3"></a> Araştırma Projesi 3

- Font family dosyası nasıl oluşturulup kullanıyoruz?
- Neden belirttiğiniz şekilde kullanımı tercih ediyoruz?

P.S. [Bu linkten](https://developer.android.com/guide/topics/ui/look-and-feel/fonts-in-xml ) faydalanarak font family projenizde deneyebilirsiniz.

Cevap:
       Bir yazı tipi ailesi stil ve ağırlık ayrıntıları ile birlikte bir yazı tipi dosya kümesidir. Bir XML kaynağı olarak yeni bir yazı tipi oluşturabilir ve bu              özellik sayesinde  her  stil ve ağrılık için ayrı kaynaklar yerine tek bir birim ile erişebiliriz. Android Studio da aşağıdaki adımları izlersek yeni bir yazı          tipi ailesi oluşturulabiliriz. Örneğin:
       ![image](https://user-images.githubusercontent.com/44816070/165764895-e12ca4b1-f276-4f8b-81f9-bbd623229637.png)
       ![image](https://user-images.githubusercontent.com/44816070/165765005-b68ef840-0c9f-46d1-a390-702b393eeb3a.png)
       ![image](https://user-images.githubusercontent.com/44816070/165765426-95cdf860-dd57-4130-987c-c8f1b0ab2070.png)


      
      

## <a name="4"></a> Araştırma Projesi 4

- Property Animation ile ilgili olarak objectAnimator ile animator arasındaki farkı kısaca açıklayınız

P.S. [Bu linkten](https://developer.android.com/guide/topics/resources/animation-resource#Property) faydalanabilirsiniz.

Cevap:
       objectAnimator belirli bir süre boyuna nesnein belirli bir özelliğini canlandırır. Animator ise belirli bir süre boyunca bir animasyon gerçekleştirir. Animator        ValueAnimator temisil eder. ObjectAnimator, valueAnimatorun bir alt sınıfıdır.
       
       Detaylı bilgi için https://developer.android.com/guide/topics/resources/animation-resource#Property sayfasını inceleyebilirsiniz.
       
