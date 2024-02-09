এই মডিউলে যা যা দেখানো হয়েছে, তার উপর ভিত্তি করে আপনাদের জন্যে এই এসাইনমেন্ট তৈরি করা হয়েছে। এই এসাইনমেন্ট এর জন্য আমরা পূর্বের মত HTML/ Tailwind CSS ব্যবহার করে একটি template তৈরি করে দিয়েছি। আপনাদেরকে এই template ব্যবহার করেই এসাইনমেন্টটি করতে হবে । HTML Template টি গিটহাবে রিপোসিটরিতে "dist" folder এর ভিতরে পেয়ে যাবেন। মনে রাখবেন, এখন পর্যন্ত যা যা দেখানো বা শেখানো হয়েছে সেগুলোর মধ্যে থেকেই আপনাকে এসাইনমেন্ট করতে হবে । আমাদের বলে দেয়া নিয়মের বাহিরে গিয়ে, আপনার মন মত করে এসাইনমেন্ট করলে কোন মার্ক দেয়া হবে না । এক্ষেত্রে কোন আর্জি শোনা হবে না । 

## এসাইনমেন্টে আপনাকে যা যা করতে হবেঃ
✓ আপনাদের News Feed এপ্লিকেশন এর টেমপ্লেট দিয়ে দেয়া হয়েছে এটিকে রিয়্যাক্টে কনভার্ট করে API থেকে নিউজ নিয়ে এসে দেখাতে হবে। এক্ষেত্রে আপনাদের আমাদের বানিয়ে দেয়া API ব্যবহার করতে হবে। আমাদের বানিয়ে দেয়া API টি কিভাবে ব্যবহার করবেন সেটি বুঝতে এসাইনমেন্ট ভিডিওটি দেখুন অথবা নিচের এই সেকশন থেকে বুঝে নিন। মনে রাখবেন, **API থেকে news নিয়ে আসতে আপনারা Fetch এর পরিবর্তে Axios বা অন্য কিছু ব্যবহার করতে পারবেন না**।

[_এই এসাইনমেন্ট এ আপনাকে .env ফাইলে কিছু তথ্য রাখতে হতে পারে । কিন্তু খেয়াল রাখবেন, .gitignore এ যেন .env ফাইল ignore করা না থাকে । অর্থাৎ, আপনি যখন github এ কোড পুশ দিবেন, তখন যেন আপনার কোডের সাথে .env ফাইল ও আপলোড হয়। যদি কোনো কারণে আপনার .env আমরা এসাইনমেন্ট চেক করার সময় না পাই, সেক্ষেত্রে আপনার এসাইনমেন্ট মার্কিং করা হবে না । এবং পরবর্তিতে আপনার ভুল সংশোধন এর ও কোনো প্রকার সুযোগ দেয়া হবে না। তবে আপনি যদি .env ফাইলে কোন তথ্য না রাখেন, সেক্ষেত্রে ব্যাপারটি আলাদা। সেক্ষেত্রে মার্ক কাটা যাবেনা। সোজা কথা, আপ্ন_] 

✓ নেভিগেশনবার এ বিভিন্ন ক্যাটেগরির নাম থাকবে, সেই নাম গুলোতে ক্লিক করলে Filter করে শুধু সেই ক্যাটেগরি এর নিউজ দেখাতে হবে । অর্থাৎ এখানে আপনাকে Filter Feature ইমপ্লিমেন্ট করতে হবে । উল্লেখ্য, আপনি চাইলে টেমপ্লেটে দেয়া ক্যাটেগরির নাম গুলো পরিবর্তন করতে পারেন । এই ক্যাটেগরির নাম আপনি API দিয়েও নিয়ে আসতে পারেন অথবা Hard Code করেও লিখতে পারেন । তবে সর্বনিম্নে পাঁচটি ক্যাটেগরি আপনাকে দেখাতেই হবে ।

✓ আপনাকে সার্চ ফিচার ইমপ্লিমেন্ট করতে হবে । এক্ষেত্রে API থেকে সার্চ করে নিয়ে এসে সার্চ রেজাল্ট দেখাতে হবে । সার্চ এর ক্ষেত্রে Debounce ব্যবহার করতে হবে । যদি Debounce সম্পর্কে না জেনে থাকেন তবে এই ভিডিও দেখে নিতে পারেন - [Debounce Function in Javascript](https://youtu.be/dD9O8DnIBj4?si=IiCCs6S9HsJl976m)

✓ আপনাকে একটি Custom Hook হুক বানাতে হবে । সেটির নাম হতে হবে **useNewsQuery** এবং সেটির কাজ হবে Fetch দিয়ে API রিকুয়েস্ট করা । আপনাদের যেই [News Api](https://newsapi.org/docs/get-started) টি দেয়া হয়েছে, সেটিতে আপনারা চাইলে Category সিলেক্ট করেও রিকুয়েস্ট করতে পারেন আবার সিলেক্ট না করেও রিকুয়েস্ট করতে পারেন । সিলেক্ট করে রিকুয়েস্ট করলে, শুধু ঐ ক্যাটেগরির নিউজ আসবে, আর সিলেক্ট না রিকুয়েস্ট করলে সব নিউজ আসবে । এখন আপনাকে হুক এমন ভাবে বানাতে হবে যেন, একটি হুক দিয়েই আপনি Categorized এবং Uncategoriezed দুই ধরণের নিউজই নিয়ে আসতে পারেন ।

✓ নেভিগেশনবার থেকে বিভিন্ন ক্যাটেগরির নিউজ দেখার ক্ষেত্রে আপনার কোড এমন ভাবে Optimized করতে হবে যেন, কোনো ক্যাটেগরির নিউজ একবার নিয়ে আসলে সেই ক্যাটেগরির নিউজ এর জন্যে পরের বার যেন API রিকুয়েস্ট **না করতে হয়** । ধরুন, প্রথমবার ইউজার যখন "Sports" ক্যাটেগরিতে যাবে, তখন একবার Sports Category এর জন্যে রিকুয়েস্ট করে ডেটা নিয়ে আসা হবে । পরের বার অন্যান্য ক্যাটেগরি ভিজিট করার পরে, আবার যদি "Sports" ক্যাটেগরিতে যাওয়া হয়, তখন যেন পুনরায় API রিকুয়েস্ট না করা হয় ।

## সামগ্রিক বিধিনিষেধঃ

- API এর জন্যে আপনি Fetch এর পরিবর্তে Axios ব্যবহার করতে পারবেন না ।
- যেহেতু Routing এখন পর্যন্ত দেখানো হয়নি, যেহেতু সেটি আপনি ব্যবহার করতে পারবেন না ।
- এই এসাইনমেন্ট এর জন্যে শুধু মাত্র পাঁচটি রিকুয়ারমেন্ট লিখে দেয়া হয়েছে, এগুলোর বাহিরেও আপনার কোডের হাইজিন ফ্যাক্টর এবং বেশ কিছু জায়গায় আমরা কিছু সমস্যা বা ইউজার এক্সপেরিয়ান্স আর ভালো করার scope রেখে দিয়েছি । সেগুলো আপনাকে implement করতে হবে এবং সেগুলো Implement এর ক্ষেত্রে আপনার কমন্সেস আমরা খেয়াল করবো । এ বিষয়ে Discord এ কোন ধরণের আলোচনা করা যাবে না ।
- আপনি চাইলে useReducer বা useContext ব্যবহার করতে পারেন ।
- কোডের স্ট্রাকচার এবং **প্রয়োজন ব্যাতিত** কোন ধরনের লিখা, ছবি, রঙ, আইকন, সাইজ বা অন্য কোন কিছুর পরিবর্তন করতে পারবেন না ।
- রিকুয়ারমেন্ট সেকশনে বলা বিষয় গুলো ব্যাতিত, "সামগ্রিক বিধিনিষেধ" সেকশনে বলা কোন বিষয় নিয়ে Discord এ প্রশ্ন করা যাবে না । বিশেষভাবে হাইজিন ফ্যাক্টর এবং আমরা যেই সমস্যা গুলো রেখেছি সে বিষয়ে জানতে চেয়ে কোন প্রশ্ন করা যাবে না ।

## কিভাবে সাবমিট করবেনঃ

সবচেয়ে সহজে বুঝার জন্য [এই ভিডিওটি](https://learnwithsumit.com/rnext/courses/rnext/how-to-submit-assignments-in-reactive-accelerator-course) দেখে ফেলুন।

এসাইনমেন্টে আপনাকে মাত্র দুইটা জিনিস সাবমিট করতে হবে।

1. **GitHub private repository link:** অবশ্যই সঠিক গিটহাব রিপোজিটরি লিংক দিতে হবে। ভুলে অন্য কোনো লিংক দিলে আপনি এসাইনমেন্টের মার্ক পাবেন না তাই সাবমিট করার আগে নিউ ট্যাবে লিংক ওপেন করে চেক করে নিবেন সঠিক লিংক জমা দিচ্ছেন কিনা।
2. **Live site link:** নেটলিফাইতে বা ভার্সেলে সাইট হোস্ট করে সাইটের লাইভ লিংক দিতে হবে। ভুলে অন্য কোনো লিংক দিলে আপনি এসাইনমেন্টের মার্ক পাবেন না তাই সাবমিট করার আগে নিউ ট্যাবে লিংক ওপেন করে চেক করে নিবেন সঠিক লিংক জমা দিচ্ছেন কিনা। নেটলিফাইতে বা ভার্সেলে কি ভাবে হোস্ট করতে হয় তা আপনি না জানলে [এইখানে ক্লিক](https://learnwithsumit.com/rnext/courses/rnext/how-to-deploy-your-project-to-vercel-free) করে দেখে নিতে পারেন।

**সাবমিট একবারই করতে পারবেন তাই ভালো করে দেখে সাবমিট করবেন।**

## GitHub private repository কিভাবে তৈরি করবেন:

Github Private repositoty তৈরি করতে [এইখানে ক্লিক করুন](https://classroom.github.com/a/4tinm3gO) অথবা ব্রাউজারে এই লিংকে **https://classroom.github.com/a/4tinm3gO** ভিজিট করুন। লিংকে যাওয়ার পরে **Accept this assignment** এ ক্লিক করুন। সর্বোচ্চ ১ মিনিট পরে পেইজটি রিলোড দিলে আপনি আপনার রিপোজেটরি লিংক পেয়ে যাবেন। মনে রাখবেন, আপনাকে এই লিংকটি আমাদের প্লাটফর্মে সাবমিট করতে হবে। না বুঝলে উপরে বলা ভিডিও টিউটোরিয়ালটি দেখে নিন।

## Assignment এর জন্য প্রয়োজনীয় template HTML:

প্রতিটি assignment এর সাথে প্রয়োজনীয় HTML template আমরা দিয়ে দিয়েছি যেন আপনাকে HTML template নিয়ে সময় নষ্ট না করতে হয়। কোর্সের GitHub repository এর সংশ্লিষ্ট ব্রাঞ্চে গেলেই আপনারা 'dist' folder এর ভিতর HTML template পাবেন। না বুঝলে [এইখানে ক্লিক](https://learnwithsumit.com/rnext/courses/rnext/how-to-submit-assignments-in-reactive-accelerator-course) করে টিউটোরিয়াল দেখে নিতে পারেন।

## এসাইনমেন্ট মার্কস পলিসি:

আপনি নির্ধারিত সময়ে এসাইনমেন্ট জমা দিলে এবং সব কিছু সঠিকভাবে করলে সম্পূর্ণ মার্ক পাবেন। এর পরে জমা দিলে আপনার মার্ক নিচের নিয়মে কাটা যাবে -

1. ডেডলাইনের পরে এক ঘণ্টার মধ্যে জমা দিলে 10% মার্ক কাটা যাবে।
2. ডেডলাইনের পরে এক ঘণ্টার বেশি কিন্তু 24 ঘণ্টার মধ্যে জমা দিলে 30% মার্ক কাটা যাবে।
3. ডেডলাইনের পরে 24 ঘণ্টার বেশি পরে জমা দিলে 50% মার্ক কাটা যাবে।
4. কোর্স ডিউরেশনের পরে আমরা এসাইনমেন্ট গ্রহণ করবো না।

অবশ্যই কোর্স চলাকালিন সময়ে এসাইনমেন্ট জমা দিতে হবে। কোর্সের ডিউরেশন শেষ হয়ে গেলে তার পরে আপনি এসাইনমেন্টে জমা দিলে এসাইনমেন্টের মার্ক পাবেন না।

## সাবমিট করার পর কোড পরিবর্তন:

আপনি ভেবে নিতে পারেন আপনি ওয়েবসাইটে সঠিক সময়ে এসাইনমেন্ট সাবমিট করে নীরবে পরে গিটহাবে কোড পুশ করতে থাকবেন! আপনার গিটহাবের সর্বশেষ কমিট দেখলেই আমরা বুঝতে পারবো আপনি কখন কোড আপডেট করেছেন। সে অনুযায়ী আমরা আপনার মার্ক কেটে নিবো। তাই এসাইনমেন্ট এর সময় পার হবার পরে আমরা আশা করবো আপনি চালাকি করে আর কোড পুশ করবেন না আপনার রিপোজিটরিতে। এটা করলে আপনার সম্পূর্ণ মার্ক কাটা যেতে পারে।

## এসাইনমেন্ট মার্কস কবে পাবেন:

আমরা সর্বোচ্চ ১৫ কার্যদিবসের ভিতরে এসাইনমেন্টের মার্ক দিয়ে দেওয়ার চেষ্টা করবো। ক্ষেত্র বিশেষে একটু দেরি হতে পারে কারো কারো মার্ক পেতে।
