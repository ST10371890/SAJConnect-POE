# SAJConnect-POE
Application that helps the youth with getting jobs (Unemployment Reducer)
# SAJConnect - Android (Kotlin) Prototype

SAJConnect helps South African youth find jobs by uploading resumes, matching skills to jobs, and applying directly.

## What's included
- Kotlin Android app (activities: Login, Profile Setup, Job Feed, Job Detail)
- Supabase / REST-ready network layer (Retrofit)
- Resume upload helper (multipart to Supabase Storage)
- Room DB skeleton & WorkManager sync skeleton
- ViewBinding enabled and logging-ready
- Unit test scaffold and GitHub Actions CI workflow

## Quick start
1. Clone repo.
2. In `local.properties` add:
SUPABASE_URL=https://<your-project>.supabase.co
SUPABASE_ANON_KEY=pk_XXXX
3. Add `google-services.json` to `app/` if using Firebase (optional).
4. Place your app icon `ic_sajconnect.png` in `app/src/main/res/mipmap-anydpi/`.
5. Open project in Android Studio, Build → Clean Project → Rebuild Project.
6. Run on emulator or device.

## Edge Functions (resume parsing)
- Deploy separately using Supabase CLI (see earlier conversation for full Node example).

## Tests & CI
- GitHub Actions workflow builds app and runs unit tests.

## Release (short)
1. Generate keystore in Android Studio or with `keytool`.
2. Build release: `./gradlew bundleRelease` (for AAB) or `assembleRelease`.
3. Sign and upload to Google Play Console.

## Demo checklist for POE
- Show app running on device/emulator.
- Register & login.
- Upload resume.
- Show parsed skills in Supabase (if Edge function used).
- Show job feed, apply to job (verify in DB).
- Show settings change (language/notifications).
- Show GitHub repo & CI passing.
- Provide unlisted YouTube demo link and include it here.

## AI usage (max 500 words)
During the development of the SAJConnect Android application, I used OpenAI’s ChatGPT as an educational and developmental assistant (OpenAI, 2025). This tool was used responsibly and in line with academic integrity standards (OpenAI, 2025). My purpose in using AI was to enhance understanding, improve productivity, and maintain professional code standards, not to replace original problem-solving or design work (OpenAI, 2025).
 
ChatGPT was specifically used for: 

-	Code Generation and Debugging Assistance: 
Guidance on writing and optimizing Kotlin code for Android Studio, including Firebase Authentication, Firestore database operations, RecyclerView adapters, and data models (OpenAI, 2025). 
Help with identifying syntax or logic errors, suggesting corrections, which I then reviewed, tested, and refined for my project (OpenAI, 2025). 
-	Layout and UI Design Suggestions: 
Drafting XML layouts for screens such as login, registration, job listings, application forms, and profile settings (OpenAI, 2025). 
These layouts were adapted to match my theme and visual preferences for consistency and usability (OpenAI, 2025). 

-	Firebase Integration and Troubleshooting: 
Explaining how to configure Firebase in Android Studio, enable Firestore, and set rules (OpenAI, 2025). 
Providing alternatives when Firebase Storage permissions caused issues, allowing for a functional prototype that behaves realistically (OpenAI, 2025). 

-	Feature Planning and Documentation Support: 
Assisting in breaking down project requirements into actionable steps, setting up version control, GitHub repository creation, integrating CI testing, and writing structured documentation (OpenAI, 2025). 

-	Learning Enhancement: 
Helping me better understand Kotlin syntax, Firebase SDK usage, and mobile app design best practices (OpenAI, 2025). 
All AI-generated content was reviewed, rewritten in my own words, and integrated only after ensuring originality and accuracy (OpenAI, 2025). 
No output from ChatGPT was used without modification or understanding (OpenAI, 2025). The final app reflects my own work and comprehension of Android app development, with AI guidance supporting clarity, speed, and structure (OpenAI, 2025). 


