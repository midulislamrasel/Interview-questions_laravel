# Laravel ইন্টারভিউ প্রস্তুতির গাইড

## পরিচিতি
এই গাইডটি Laravel ইন্টারভিউ প্রস্তুতির জন্য প্রশ্ন ও উত্তরগুলির একটি সংগ্রহ প্রদান করে। এটি Laravel এর বৈশিষ্ট্য, সেরা অভ্যাস এবং উন্নত বিষয়গুলি কভার করে।

## মৌলিক প্রশ্ন

1. **Laravel কী?**
   Laravel একটি PHP ফ্রেমওয়ার্ক যা MVC (Model-View-Controller) আর্কিটেকচার ব্যবহার করে, যা ওয়েব অ্যাপ্লিকেশন ডেভেলপমেন্টকে সহজ এবং দ্রুত করে তোলে।

2. **Laravel এর প্রধান বৈশিষ্ট্যগুলো কী কী?**
   - রাউটিং
   - ORM (Eloquent)
   - Middleware
   - Authentication
   - Artisan Command Line Interface
   - Blade Templating Engine
   - Laravel Mix

3. **Routes ফাইলগুলোর ভূমিকা কী?**
   Routes ফাইলগুলো HTTP রিকোয়েস্ট কিভাবে প্রক্রিয়া করা হবে তা নির্ধারণ করে। সাধারণত এগুলি `routes/web.php` এবং `routes/api.php` এ থাকে।

4. **Eloquent ORM কী?**
   Eloquent হল Laravel এর ইন-বিল্ট ORM সিস্টেম যা মডেল ক্লাসের মাধ্যমে ডাটাবেস টেবিলগুলির সাথে যোগাযোগ করতে দেয় এবং সরাসরি SQL কোড লেখার প্রয়োজনীয়তা কমায়।

5. **Middleware কী?**
   Middleware হল একটি ফিল্টার যা HTTP রিকোয়েস্ট এবং রেসপন্সের মধ্যে অবস্থান করে, যেমন অথেনটিকেশন বা লগিং।

6. **Service Providers কী?**
   Service Providers হল Laravel এর মূল কনফিগারেশন পয়েন্ট যা সার্ভিস কনটেইনারের মধ্যে ডিপেনডেন্সি ইনজেকশন এবং সার্ভিস রেজিস্ট্রেশন করে।

7. **Blade Templating Engine কী?**
   Blade হল Laravel এর টেমপ্লেট ইঞ্জিন যা ডাইনামিক কন্টেন্ট পেজে প্রদর্শনের জন্য ব্যবহৃত হয় এবং PHP কোড লেখার সুবিধা দেয়।

8. **Laravel এর Migration কী?**
   Migration একটি টুল যা ডাটাবেস স্কিমা তৈরি এবং পরিচালনা করতে সাহায্য করে এবং এটি ডাটাবেস পরিবর্তনসমূহ ট্র্যাক করার জন্য ব্যবহৃত হয়।

9. **Laravel এর Jobs এবং Queues কী?**
   Jobs এবং Queues ব্যাকগ্রাউন্ড টাস্ক প্রক্রিয়া করার জন্য ব্যবহৃত হয়, যা লম্বা সময়ের প্রক্রিয়া বা কাজগুলো অ্যাসিঙ্ক্রোনাস ভাবে চালায়।

10. **Laravel এর Testing কী?**
    Laravel ইন-বিল্ট টেস্টিং ফিচার সরবরাহ করে যেমন ইউনিট টেস্টিং এবং ফিচার টেস্টিং, যা অ্যাপ্লিকেশন কোডের মান যাচাই করতে ব্যবহৃত হয়।

## মধ্যবর্তী প্রশ্ন

11. **Route Model Binding কী?**
    Route Model Binding আপনাকে রাউটগুলিতে মডেল ইনস্ট্যান্স সরাসরি পাস করতে দেয়, যেমন `Route::get('/user/{user}', function (User $user) { ... });`।

12. **Laravel এ Dependency Injection কীভাবে কাজ করে?**
    Laravel এর সার্ভিস কনটেইনার ডিপেনডেন্সি ইনজেকশন পরিচালনা করে, যা ক্লাসের ইনস্ট্যান্স তৈরি এবং ডিপেনডেন্সি রেজিস্টার করে।

13. **Laravel এ Custom Validation Rules কীভাবে তৈরি করবেন?**
    Custom Validation Rules তৈরি করতে, আপনি Laravel এর `Illuminate\Contracts\Validation\Rule` ইন্টারফেস ইমপ্লিমেন্ট করে একটি কাস্টম রুল ক্লাস তৈরি করতে পারেন।

14. **Laravel এ Session কীভাবে পরিচালনা করবেন?**
    Laravel বিভিন্ন ড্রাইভার ব্যবহার করে সেশন পরিচালনা করে, যেমন ফাইল, কুকি, ডাটাবেস। সেশন পরিচালনার জন্য আপনি `config/session.php` ফাইলে কনফিগারেশন সেট করতে পারেন।

15. **Laravel এ Queue কাজ কীভাবে করে?**
    Queue পদ্ধতি ব্যাকগ্রাউন্ড টাস্ক প্রক্রিয়া করতে ব্যবহৃত হয়। আপনি কাজগুলো (Jobs) তৈরি করেন এবং সেগুলোকে Queue তে পুশ করেন। পরে Queue Worker কাজগুলো প্রক্রিয়া করে।

16. **Laravel এ Policies এবং Gates কী?**
    Policies এবং Gates হল অথোরাইজেশন মেকানিজম যা নির্দিষ্ট অ্যাকশনগুলোর জন্য ইউজারের অনুমোদন যাচাই করতে ব্যবহৃত হয়। Policies ক্লাসে অথোরাইজেশন লজিক রাখে, এবং Gates সিম্পল ক্লোজার ফাংশন হিসেবে ব্যবহৃত হয়।

17. **Laravel এ Events এবং Listeners কীভাবে কাজ করে?**
    Events এবং Listeners হল Laravel এর ইভেন্ট-ড্রিভেন আর্কিটেকচার অংশ। আপনি একটি ইভেন্ট ট্রিগার করতে পারেন এবং সেই ইভেন্টের জন্য এক বা একাধিক লিসনার কাজ করবে।

18. **Laravel এ Localization কী?**
    Localization হল বিভিন্ন ভাষায় অ্যাপ্লিকেশন কনটেন্ট প্রদর্শনের প্রক্রিয়া। আপনি `resources/lang` ফোল্ডারে ভাষার ফাইল রাখেন এবং `__()` বা `@lang` ফাংশন ব্যবহার করে ভাষার কনটেন্ট রিটারিভ করতে পারেন।

19. **Laravel এর `artisan` কমান্ড কী?**
    Artisan হল Laravel এর কমান্ড লাইন ইন্টারফেস যা ডেভেলপমেন্ট কাজ সহজ করার জন্য বিভিন্ন কমান্ড প্রদান করে, যেমন `php artisan make:controller`, `php artisan migrate`, ইত্যাদি।

20. **Laravel এ Caching কীভাবে কনফিগার করবেন?**
    Caching হল ডেটা দ্রুত পাওয়ার জন্য ক্যাশ মেকানিজম ব্যবহার করা। Laravel বিভিন্ন ক্যাশ ড্রাইভার সমর্থন করে, যেমন `file`, `redis`, `memcached`। ক্যাশ ব্যবহার করার জন্য `Cache` ফেসাড ব্যবহার করা হয়।

## উন্নত প্রশ্ন

21. **Migrations এবং Seeders এর মধ্যে পার্থক্য কী?**
    - **Migrations:** ডাটাবেস স্কিমা পরিবর্তনের জন্য ব্যবহৃত হয়।
    - **Seeders:** ডাটাবেসে প্রাথমিক ডাটা পূরণের জন্য ব্যবহৃত হয়।

22. **Laravel এ Dependency Injection কীভাবে কাজ করে?**
    Laravel এর সার্ভিস কনটেইনার ব্যবহার করে Dependency Injection করা হয়। এটি ক্লাসের ইনস্ট্যান্স তৈরি এবং ডিপেনডেন্সি রেজিস্টার করে, যা কোডের মডুলারিটি এবং টেস্টেবিলিটি বৃদ্ধি করে।

23. **API Resources কীভাবে ব্যবহার করবেন?**
    API Resources JSON রেসপন্সের ফরম্যাট কাস্টমাইজ করতে সহায়তা করে। `php artisan make:resource` কমান্ড দিয়ে একটি রিসোর্স ক্লাস তৈরি করে এবং `toArray` মেথডে ডাটা কাস্টমাইজ করা হয়।

24. **Service Container কী?**
    Service Container হল একটি কনটেইনার যা ডিপেনডেন্সি ইনজেকশন এবং সার্ভিস রেজিস্ট্রেশন পরিচালনা করে। এটি ক্লাসের ইনস্ট্যান্স তৈরি এবং ডিপেনডেন্সি রেজিস্টার করে।

25. **CORS কিভাবে কনফিগার করবেন?**
    CORS (Cross-Origin Resource Sharing) কনফিগার করার জন্য, Laravel এ `fruitcake/laravel-cors` প্যাকেজ ব্যবহার করা হয়। এটি `config/cors.php` ফাইলে কনফিগারেশন করতে দেয়।

26. **Custom Exception Handling কিভাবে করবেন?**
    কাস্টম এক্সসেপশন হ্যান্ডলিংয়ের জন্য, আপনি `App\Exceptions\Handler` ক্লাসে `render` বা `report` মেথডে কাস্টম লজিক যোগ করতে পারেন।

27. **Policy ক্লাস কিভাবে তৈরি করবেন?**
    Policy ক্লাস তৈরি করতে `php artisan make:policy` কমান্ড ব্যবহার করুন। এরপর, রেজিস্ট্রেশন করতে `AuthServiceProvider` এ যোগ করুন।

28. **Static Method কিভাবে ব্যবহার করবেন?**
    Static Method সাধারণত ক্লাসে `static` কীওয়ার্ড ব্যবহার করে তৈরি করা হয়। Laravel এ Static Method ব্যবহার করার সময়, মনে রাখতে হবে যে Dependency Injection সাপোর্ট করা হয় না।

29. **`DB::transaction` মেথড কিভাবে কাজ করে?**
    `DB::transaction` মেথড ডাটাবেস ট্রানজেকশন পরিচালনা করে। এটি নিশ্চিত করে যে একটি ব্লক কোড সম্পূর্ণ সফল হলে ডাটাবেসে পরিবর্তনসমূহ সংরক্ষিত হবে, অন্যথায় পরিবর্তনসমূহ বাতিল হবে।

30. **পাসওয়ার্ড হ্যাশিং কিভাবে করবেন?**
    Laravel এ পাসওয়ার্ড হ্যাশিং করতে `bcrypt` বা `Hash` ফেসাড ব্যবহার করা হয়। উদাহরণস্বরূপ: `Hash::make('password')`।

## অতিরিক্ত প্রশ্ন

31. **Subqueries কিভাবে ব্যবহার করবেন?**
    Laravel এর Eloquent এবং Query Builder এ সাবকোয়েরি ব্যবহার করতে `DB::table` বা `Model::select` এর মধ্যে সাবকোয়েরি ব্যবহার করা যায়।

32. **Artisan Command কিভাবে তৈরি করবেন?**
    নতুন Artisan কমান্ড তৈরি করতে `php artisan make:command` কমান্ড ব্যবহার করুন। এরপর, কমান্ডের লজ
    কাস্টম লজিক `app/Console/Commands` ডিরেক্টরিতে আপনার কমান্ড ক্লাসে যুক্ত করুন।

33. **Mail Sending কিভাবে করবেন?**
    Laravel এ মেইল পাঠানোর জন্য `Illuminate\Support\Facades\Mail` ফেসাড ব্যবহার করা হয়। আপনি `php artisan make:mail` কমান্ড দিয়ে একটি মেইল ক্লাস তৈরি করতে পারেন এবং `Mail::to($recipient)->send(new YourMailableClass());` ব্যবহার করে মেইল পাঠাতে পারেন।

34. **Blade Components কিভাবে তৈরি করবেন?**
    Blade Components তৈরি করতে `php artisan make:component ComponentName` কমান্ড ব্যবহার করুন। তারপর, কম্পোনেন্ট ফাইল এবং ভিউ তৈরি হবে `app/View/Components` এবং `resources/views/components` এ।

35. **Task Scheduling কিভাবে কাজ করে?**
    Task Scheduling ব্যবহারের জন্য `app/Console/Kernel.php` ফাইলে `schedule` মেথডে আপনার টাস্কগুলো ডিফাইন করতে হয়। উদাহরণস্বরূপ:
    ```php
    protected function schedule(Schedule $schedule)
    {
        $schedule->command('inspire')->hourly();
    }
    ```

36. **Data Caching কিভাবে কাজ করে?**
    ডাটা ক্যাশিং করতে `Cache` ফেসাড ব্যবহার করা হয়। উদাহরণস্বরূপ:
    ```php
    Cache::put('key', 'value', $minutes);
    $value = Cache::get('key');
    ```

37. **Event Broadcasting কিভাবে কাজ করে?**
    Event Broadcasting ব্যবহার করতে, প্রথমে `Event` তৈরি করতে হয় এবং তারপর `broadcastOn` মেথড ব্যবহার করে চ্যানেল নির্ধারণ করতে হয়। এরপর, ক্লায়েন্ট সাইডে পুশ নোটিফিকেশন বা আপডেট দেখানোর জন্য লাইভওয়্যার অথবা পুশার লাইব্রেরি ব্যবহার করতে হয়।

38. **Custom Helper Functions কিভাবে যুক্ত করবেন?**
    কাস্টম হেল্পার ফাংশন যুক্ত করতে `app/helpers.php` ফাইল তৈরি করতে পারেন এবং `composer.json` এর `autoload` অংশে ফাইলটি যুক্ত করতে পারেন। উদাহরণস্বরূপ:
    ```json
    "files": [
        "app/helpers.php"
    ]
    ```

39. **Job Chaining কিভাবে ব্যবহার করবেন?**
    Job Chaining ব্যবহার করতে আপনি একটি জবের `chain` মেথড ব্যবহার করতে পারেন যা একাধিক জবকে একসাথে কার্যকর করে। উদাহরণস্বরূপ:
    ```php
    Job1::withChain([
        new Job2,
        new Job3
    ])->dispatch();
    ```

40. **Form Requests কিভাবে ব্যবহার করবেন?**
    Form Requests হল একটি ক্লাস যা ইনপুট ভ্যালিডেশন এবং অথোরাইজেশন লজিক ধারণ করে। `php artisan make:request RequestName` কমান্ড ব্যবহার করে একটি ফর্ম রিকোয়েস্ট ক্লাস তৈরি করুন এবং কন্ট্রোলারে টাইপহিনিং ব্যবহার করে ইনজেক্ট করুন।

## উপসংহার
এই গাইডটি Laravel এর বিভিন্ন বিষয় কভার করে। এই ধারণাগুলো আপনার Laravel সম্পর্কিত ইন্টারভিউ প্রস্তুতির জন্য সহায়ক হবে।
