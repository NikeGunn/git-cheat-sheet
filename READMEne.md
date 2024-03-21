गिट कमान्डश
============

## अनुवादित संस्करण
- [नेपाली अनुवाद](READMEne.md)
___

_बिसेशरी उपयोग गरिने गिट कमांड का सूची_

*यदि तपाईं गिट उपनाम मा रुचि , रख्नुहुछ भने `.bash_profile` यहाँ जानुस : https://github.com/NikeGunn/git-cheat-sheet/blob/main/.bash_profile*

--

### प्रोजेक्ट प्राप्त गर्ने अनि बनाउने 

| कमान्ड | विवरण |
| ----- | ----- |
| `git init` | लोकल गिट रिपॉजिटरी लाई इनिशियलाइज़ गरौं |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | आफ्नो रिपॉजिटरी को एक लोकल कॉपी बनाउँ |

### बेसिक स्नैपशॉटिंग

| कमान्ड | विवरण |
| ----- | ----- |
| `git status` | स्टेटस जाचौँ |
| `git add [file-name.txt]` | फ़ाइल को स्टेजिंग एरिया जोडौं |
| `git add -A` | सपैँ नयाँ अनि परिवर्तित फ़ाइल को स्टेजिंग एरिया जोडौं |
| `git commit -m "[commit message]"` | चैन्जश को मेसज को साथ कमिट गरौं |
| `git rm -r [file-name.txt]` | एक फ़ाइल (या फ़ोल्डर) निकालौं |

### ब्रान्चिंग अनि मर्जिंग

| कमान्ड | विवरण |
| ----- | ----- |
| `git branch` | ब्रांचश को सूची बनाऊँ (ऐस्टरिस्क[*] साइन वर्तमान शाखा लाई दर्साउछ ) |
| `git branch -a` | सपैँ ब्रांचश अनि सूची बनाऊँ (लोकल अनि रिमोट) |
| `git branch [branch name]` | एक नयाँ ब्रांच बनाऊँ |
| `git branch -d [branch name]` | एक ब्रांच डिलीट गरौं |
| `git push origin --delete [branch name]` | एक रिमोट ब्रांच हटाओं |
| `git checkout -b [branch name]` | एक नयाँ ब्रांच बनाओं अनि तेस्मा स्विच गरौं |
| `git checkout -b [branch name] origin/[branch name]` | एक रिमोट ब्रांच को क्लोन गरौं अनि तेस्मा स्विच गरौं |
| `git branch -m [old branch name] [new branch name]` | एक रिमोट ब्रांच का नाम बदलौँ |
| `git checkout [branch name]` | एक ब्रांच मा स्विच गरौं |
| `git checkout -` | पछील्लो चोटी चेक आउट गरिएको ब्रांच मा स्विच गरौं |
| `git checkout -- [file-name.txt]` | कुनै एक फ़ाइल मा सपैँ परिवर्तन निकलौँ |
| `git merge [branch name]` | एक ब्रांच को ऐक्टिव ब्रांच मा मर्ज गरौं |
| `git merge [source branch] [target branch]` | एक ब्रांच को टार्गेट ब्रांच मा मर्ज गरौं |
| `git stash` | वर्किंग फोल्डर मा चैन्जश को स्टैश गरौं |
| `git stash clear` | सपैँ स्टैश चैन्जश हटाओं ( clear ) |

### प्राजेक्ट्स लाई शेर अनि अप्डेट गर्ने तरिका 

| कमान्ड | विवरण |
| ----- | ----- |
| `git push origin [branch name]` | अपने रिमोट रिपॉजिटरी मा ब्रांच लाई पुश गरौं |
| `git push -u origin [branch name]` | रिमोट रिपॉजिटरी मा ब्रांच लाई पुश गरौं (अनि तेइ ब्रांच लाई याद राखौं) |
| `git push` | रिमोट रिपॉजिटरी मा ब्रांच लाई पुश गरौं (तेई याद रखिएको ब्रांच मा) |
| `git push origin --delete [branch name]` | एक रिमोट ब्रांच लाई डिलीट गरौं |
| `git pull` | आफ्नो लोकल रिपॉजिटरी लाई लेटेस्ट कमिट मा अपडेट गरौं |
| `git pull origin [branch name]` | रिमोट रिपॉजिटरी देखिँ चैन्जश पुल गरौं |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | एक रिमोट रिपॉजिटरी जोडौं |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | रिपॉजिटरी को ओरिजिन ब्रांच को SSH मा सेट गरौं |

### निरीक्षण और तुलना

| कमान्ड | विवरण |
| ----- | ----- |
| `git log` | चैन्जश हेरौँ |
| `git log --summary` | चैन्जश हेरौँ (डीटेल मा) |
| `git log --oneline` | चैन्जश हेरौँ (संक्षेप मा) |
| `git diff [source branch] [target branch]` | मर्जिंग भन्दा पहिले चैन्जश को समीक्षा गरौं |
