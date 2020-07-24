# AndroidLogin

Debug

2020-07-24 23:47:38.687 24344-24344/? I/e.example.urbe: Not late-enabling -Xcheck:jni (already on)
2020-07-24 23:47:38.703 24344-24344/? W/e.example.urbe: Unexpected CPU variant for X86 using defaults: x86
2020-07-24 23:47:41.037 24344-24344/? W/e.example.urbe: Current dex file has more than one class in it. Calling RetransformClasses on this class might fail if no transformations are applied to it!
2020-07-24 23:47:41.037 24344-24344/? I/chatty: uid=10099(de.example.urbex) re-initialized> identical 13 lines
2020-07-24 23:47:41.037 24344-24344/? W/e.example.urbe: Current dex file has more than one class in it. Calling RetransformClasses on this class might fail if no transformations are applied to it!
2020-07-24 23:47:41.050 24344-24344/? W/e.example.urbe: Class android.os.PowerManager$WakeLock failed lock verification and will run slower.
2020-07-24 23:47:41.050 24344-24344/? W/e.example.urbe: Common causes for lock verification issues are non-optimized dex code
2020-07-24 23:47:41.050 24344-24344/? W/e.example.urbe: and incorrect proguard optimizations.
2020-07-24 23:47:41.208 24344-24344/de.example.urbex W/e.example.urbe: Changing class Landroidx/fragment/app/Fragment;
2020-07-24 23:47:41.209 24344-24344/de.example.urbex W/e.example.urbe: Dex file created by class-definition time transformation of Landroidx/fragment/app/Fragment; is not checked for all retransformation invariants.
2020-07-24 23:47:41.289 24344-24344/de.example.urbex W/e.example.urbe: Accessing hidden method Landroid/graphics/drawable/Drawable;->getOpticalInsets()Landroid/graphics/Insets; (light greylist, linking)
2020-07-24 23:47:41.289 24344-24344/de.example.urbex W/e.example.urbe: Accessing hidden field Landroid/graphics/Insets;->left:I (light greylist, linking)
2020-07-24 23:47:41.289 24344-24344/de.example.urbex W/e.example.urbe: Accessing hidden field Landroid/graphics/Insets;->right:I (light greylist, linking)
2020-07-24 23:47:41.289 24344-24344/de.example.urbex W/e.example.urbe: Accessing hidden field Landroid/graphics/Insets;->top:I (light greylist, linking)
2020-07-24 23:47:41.289 24344-24344/de.example.urbex W/e.example.urbe: Accessing hidden field Landroid/graphics/Insets;->bottom:I (light greylist, linking)
2020-07-24 23:47:41.432 24344-24344/de.example.urbex W/e.example.urbe: Accessing hidden method Landroid/view/View;->computeFitSystemWindows(Landroid/graphics/Rect;Landroid/graphics/Rect;)Z (light greylist, reflection)
2020-07-24 23:47:41.432 24344-24344/de.example.urbex W/e.example.urbe: Accessing hidden method Landroid/view/ViewGroup;->makeOptionalFitsSystemWindows()V (light greylist, reflection)
2020-07-24 23:47:41.441 24344-24344/de.example.urbex W/e.example.urbe: Accessing hidden method Landroid/widget/TextView;->getTextDirectionHeuristic()Landroid/text/TextDirectionHeuristic; (light greylist, linking)
2020-07-24 23:47:41.489 24344-24344/de.example.urbex W/e.example.urbe: Changing class Lokhttp3/OkHttpClient;
2020-07-24 23:47:41.489 24344-24344/de.example.urbex W/e.example.urbe: Dex file created by class-definition time transformation of Lokhttp3/OkHttpClient; is not checked for all retransformation invariants.
2020-07-24 23:47:41.493 24344-24344/de.example.urbex W/e.example.urbe: Accessing hidden method Ljava/lang/invoke/MethodHandles$Lookup;-><init>(Ljava/lang/Class;I)V (light greylist, reflection)
2020-07-24 23:47:41.522 24344-24344/de.example.urbex D/AndroidRuntime: Shutting down VM
2020-07-24 23:47:41.524 24344-24344/de.example.urbex E/AndroidRuntime: FATAL EXCEPTION: main
    Process: de.example.urbex, PID: 24344
    java.lang.BootstrapMethodError: Exception from call site #4 bootstrap method
        at okhttp3.internal.Util.<clinit>(Util.java:87)
        at okhttp3.internal.Util.skipLeadingAsciiWhitespace(Util.java:321)
        at okhttp3.HttpUrl$Builder.parse(HttpUrl.java:1313)
        at okhttp3.HttpUrl.get(HttpUrl.java:917)
        at retrofit2.Retrofit$Builder.baseUrl(Retrofit.java:506)
        at de.example.urbex.ApiClient.getApiClient(ApiClient.java:17)
        at de.example.urbex.MainActivity.onCreate(MainActivity.java:18)
        at android.app.Activity.performCreate(Activity.java:7136)
        at android.app.Activity.performCreate(Activity.java:7127)
        at android.app.Instrumentation.callActivityOnCreate(Instrumentation.java:1271)
        at android.app.ActivityThread.performLaunchActivity(ActivityThread.java:2893)
        at android.app.ActivityThread.handleLaunchActivity(ActivityThread.java:3048)
        at android.app.servertransaction.LaunchActivityItem.execute(LaunchActivityItem.java:78)
        at android.app.servertransaction.TransactionExecutor.executeCallbacks(TransactionExecutor.java:108)
        at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:68)
        at android.app.ActivityThread$H.handleMessage(ActivityThread.java:1808)
        at android.os.Handler.dispatchMessage(Handler.java:106)
        at android.os.Looper.loop(Looper.java:193)
        at android.app.ActivityThread.main(ActivityThread.java:6669)
        at java.lang.reflect.Method.invoke(Native Method)
        at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:493)
        at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:858)
     Caused by: java.lang.ClassCastException: Bootstrap method returned null
        at okhttp3.internal.Util.<clinit>(Util.java:87) 
        at okhttp3.internal.Util.skipLeadingAsciiWhitespace(Util.java:321) 
        at okhttp3.HttpUrl$Builder.parse(HttpUrl.java:1313) 
        at okhttp3.HttpUrl.get(HttpUrl.java:917) 
        at retrofit2.Retrofit$Builder.baseUrl(Retrofit.java:506) 
        at de.example.urbex.ApiClient.getApiClient(ApiClient.java:17) 
        at de.example.urbex.MainActivity.onCreate(MainActivity.java:18) 
        at android.app.Activity.performCreate(Activity.java:7136) 
        at android.app.Activity.performCreate(Activity.java:7127) 
        at android.app.Instrumentation.callActivityOnCreate(Instrumentation.java:1271) 
        at android.app.ActivityThread.performLaunchActivity(ActivityThread.java:2893) 
        at android.app.ActivityThread.handleLaunchActivity(ActivityThread.java:3048) 
        at android.app.servertransaction.LaunchActivityItem.execute(LaunchActivityItem.java:78) 
        at android.app.servertransaction.TransactionExecutor.executeCallbacks(TransactionExecutor.java:108) 
        at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:68) 
        at android.app.ActivityThread$H.handleMessage(ActivityThread.java:1808) 
        at android.os.Handler.dispatchMessage(Handler.java:106) 
        at android.os.Looper.loop(Looper.java:193) 
        at android.app.ActivityThread.main(ActivityThread.java:6669) 
        at java.lang.reflect.Method.invoke(Native Method) 
        at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:493) 
        at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:858) 
