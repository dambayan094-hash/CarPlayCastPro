# CarPlay Cast Pro — iOS IPA build

ئەم project ـە React + Vite ـە و بە Capacitor دەکرێتە native iOS app.

## گرنگ
Browser ناتوانێت executable ـی iOS دروست بکات. بۆیە ئەم project ـە هیچ IPA ـی fake دروست ناکات.

### بێ Mac
GitHub Actions workflow ـەکە لە `macos-latest` runner ـی GitHub کار دەکات:

1. Repository ـەکە لە GitHub دروست بکە.
2. ناوەڕۆکی ئەم project ـە لە root ـی repository upload بکە.
3. `Actions` → `Build iOS IPA` هەڵبژێرە.
4. `Run workflow` بکە.
5. دوای تەواوبوون، لە `Artifacts` فایلەکەی `CarPlayCastPro-IPA` دابەزێنە.
6. IPA ـەکە native iOS binary ـی Mach-O هەیە و unsigned ـە؛ دواتر دەتوانیت بە شێوازی sideload ـکردنی خۆت sign بکەیت، ئەگەر signing requirements ـەکانت پڕ بکرێن.

## تێبینی CarPlay
Capacitor تەنها web app ـەکە دەخاتە ناو native iOS container. ئەمە بەخۆیەوە مۆڵەتی Apple بۆ screen mirroring یان CarPlay private APIs زیاد ناکات. بۆ CarPlay ـی ڕاستەقینە پێویستی بە APIs/entitlements ـی ڕێگەپێدراوی Apple هەیە.
