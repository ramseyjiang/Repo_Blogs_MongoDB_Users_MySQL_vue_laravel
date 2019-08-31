<h5>The following link is the aws address for this project, http://13.210.14.131/figtest/public/index.php</h5>

<h5>User Story: 1. The default page is the bloglist page, whether a user login or not, the blogs always show; 2. If a user login, he only can create, update, delete his own blogs; 3. If a user does not login, he only can view blogs. 4. If an admin user login, he can create, update, delete all users blogs. </h5>

<h5>The admin user's username is admin, user's email is admin@qq.com, password is 12345678. You can use username or email to login</h5>

<h5>The test user's username is test, user's email is test@qq.com, password is 12345678. You can use username or email to login</h5>

<h4>This project is built backend by Laravel and frontend by Vue. Users tabls is used MYSQL still, Blogs Table is used MongoDB. Both frontend and backend have been built unittests. Backend unittest is built by phpunit. Frontend unittest is built by Jest. The Laravel passport is included in this project, the whole project uses Repository pattern. </h4>

<p>If want to run this project directly, please using the following steps.</p>
<p>Step1: clone the project to your local first.</p>
<p>Step2: composer install</p>
<p>Step3: cp .env.example .env</p>
<p>Step4: php artisan key:generate</p>
<p>Step5: php artisan migrate</p>
<p>Step6: php artisan passport:install</p>
<p>Step7: php artisan db:seed --class UsersTableSeeder</p>
<p>Step8: ./vendor/bin/phpunit (It is used to run php unittests)</p>
<p>If unittests run no issues, it is fine.</p>

<p>Step9: npm install</p>
<p>Step10: npm run dev</p>
<p>Step11: npm run test</p>
<p>If all tests are no issues, it is finished.</p>

----------------------------------------------------------------------------------------------------------------------------------------

<h4>If you wanna to learn how to do this project step by step, you can follow steps under below.</h4>
<p>This readme only describes how to install and config this project, if you wanna to know the base platform how to build it, please follow this link "https://github.com/ramseyjiang/Repo_pattern_laravel_passport_vue_fullstack"</p>

<p>All steps under below are base on the fullstack you have learnt.</p>

<p>Step0: git clone https://github.com/ramseyjiang/Repo_pattern_laravel_passport_vue_fullstack project_name </p>

<p>Step1: rm -rf .git (It is used to remove all git history.)</p>

<p>Step2: composer install</p>

<p>Step3: cp .env.example .env </p>

<p>Step4: modify the database, root, password in the .env file. modify config/database.php, update the MongoDb config the same with your local.</p>

<p>Step5: php artisan key:generate</p>

<p>Step6: php artisan passport:install</p>

<p>Step7: php artisan migrate</p>

<p>Step8: php artisan db:seed --class UserTableSeeder</p>

<p>Step9: ./vendor/bin/phpunit  (To make sure the backend works, then you can use "php artisan app:name AppName" to change app name or not, it is up to you.)</p>

<p>Step10: composer require jenssegers/mongodb </p>

<p>Step11: php artisan make:controller BlogController --resource (It will generate BlogController and some default methods)</p>

<p>Step12: php artisan make:request BlogRequest (It will generate BlogRequest in a requests folder)</p>

<p>Step13: php artisan make:model Models/Log -m (It will generate Log.php within the Models folder and generate a new file in the database/migrations folder, you should fill the table content.)</p>

<p>Step14: php artisan make:model Models/Blog (It will generate a Blog model within the Models folder.)</p>

<p>Step15: php artisan make:policy BlogPolicy (It will generate a BlogPolicy file in the policies folder.)</p>

<p>Step16: php artisan make:observer BlogObserver (It will generate a BlogObserver file in the Observers folder)</p>

<p>Step17: php artisan make:test BlogTest (It will generate a BlogTest file in the tests/Feature folder.)</p>

<p>Step18: create Blog/List.vue, Blog/Edit.vue in the resources/js/components folder, create Blog/List.test.js, Blog/Edit.test.js in the resources/js/tests folder</p>

<p>Step19: Update routes.js</p>

<p>After all steps above, you can copy code from each matches file content from this project file.</p>
<p>Run "npm run dev" to compile, after that run "npm run test" to test whether frontend works or not. </p>
<p>If all the above works, this project works. Thanks for your time. If you like this project, please add a star for me. Thanks and cheers.</p>