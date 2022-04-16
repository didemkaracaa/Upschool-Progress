# Araştırma Ödevleri:

- [Araştırma Projesi 1 - Lateinit](#1)
- [Araştırma Projesi 2 - Tools Namespace](#2)


### <a name="1"></a> Araştırma Projesi 1

- Lateinit neden kullanıyoruz?
- Lateinit kullanımından bahseder misiniz?
- Lateinit için bir örnek kullanım gösterir misiniz ?
      
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

       Bir uygulama geliştirirken layout dizini içinde kullandıpımız xml dosyasını tool attribute(tools namespace) ile mümkündür. 
       Tasarım tarafında yapılan değişkenlerin çıktısını uygulamayı çalıştırmadan direk görebilmemizi sağlamaktadır. 
       Tasarım özelliklerini veya derleme zaman davranışlarını etkinleştiren XML özelliklerini destekler.
       Kullanabilmemiz için activity_main.xml dosyamız içinde "xmlns:tools="http://schemas.android.com/tools"" tanımlamamız gerekmektedir.
       Örnek vermek gerekirse:
       -Tools namespace kullanmadan
       android:text="Get unlimited"
       -Tools kullanarak
       tools:text="Get unlimited"
