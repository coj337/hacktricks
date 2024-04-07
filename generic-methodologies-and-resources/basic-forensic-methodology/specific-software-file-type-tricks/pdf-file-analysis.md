# Analiza pliku PDF

<details>

<summary><strong>Naucz się hakować AWS od zera do bohatera z</strong> <a href="https://training.hacktricks.xyz/courses/arte"><strong>htARTE (HackTricks AWS Red Team Expert)</strong></a><strong>!</strong></summary>

Inne sposoby wsparcia HackTricks:

* Jeśli chcesz zobaczyć swoją **firmę reklamowaną w HackTricks** lub **pobrać HackTricks w formacie PDF**, sprawdź [**PLAN SUBSKRYPCYJNY**](https://github.com/sponsors/carlospolop)!
* Kup [**oficjalne gadżety PEASS & HackTricks**](https://peass.creator-spring.com)
* Odkryj [**Rodzinę PEASS**](https://opensea.io/collection/the-peass-family), naszą kolekcję ekskluzywnych [**NFT**](https://opensea.io/collection/the-peass-family)
* **Dołącz do** 💬 [**grupy Discord**](https://discord.gg/hRep4RUj7f) lub [**grupy telegramowej**](https://t.me/peass) lub **śledź** nas na **Twitterze** 🐦 [**@hacktricks\_live**](https://twitter.com/hacktricks\_live)**.**
* **Podziel się swoimi sztuczkami hakerskimi, przesyłając PR-y do** [**HackTricks**](https://github.com/carlospolop/hacktricks) i [**HackTricks Cloud**](https://github.com/carlospolop/hacktricks-cloud) repozytoriów na GitHubie.

</details>

<figure><img src="../../../.gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure>

\
Użyj [**Trickest**](https://trickest.com/?utm\_campaign=hacktrics\&utm\_medium=banner\&utm\_source=hacktricks), aby łatwo budować i **automatyzować workflowy** zasilane przez najbardziej zaawansowane narzędzia społecznościowe na świecie.\
Zdobądź dostęp już dziś:

{% embed url="https://trickest.com/?utm_campaign=hacktrics&utm_medium=banner&utm_source=hacktricks" %}

**Aby uzyskać dalsze szczegóły, sprawdź:** [**https://trailofbits.github.io/ctf/forensics/**](https://trailofbits.github.io/ctf/forensics/)

Format PDF jest znany złożoności i potencjału ukrywania danych, co czyni go punktem centralnym wyzwań z zakresu forensyki CTF. Łączy on elementy tekstu z obiektami binarnymi, które mogą być skompresowane lub zaszyfrowane, i może zawierać skrypty w językach takich jak JavaScript lub Flash. Aby zrozumieć strukturę PDF, można odnieść się do materiałów wstępnych Didiera Stevensa [tutaj](https://blog.didierstevens.com/2008/04/09/quickpost-about-the-physical-and-logical-structure-of-pdf-files/), lub skorzystać z narzędzi takich jak edytor tekstu lub edytor specyficzny dla PDF, takiego jak Origami.

Dla dogłębnego badania lub manipulacji plików PDF dostępne są narzędzia takie jak [qpdf](https://github.com/qpdf/qpdf) i [Origami](https://github.com/mobmewireless/origami-pdf). Ukryte dane w plikach PDF mogą być ukryte w:

* Niewidocznych warstwach
* Formacie metadanych XMP firmy Adobe
* Generacjach inkrementalnych
* Tekście o tym samym kolorze co tło
* Tekście za obrazami lub nakładających się na obrazy
* Komentarzach niewyświetlanych

Dla niestandardowej analizy plików PDF można użyć bibliotek Pythona, takich jak [PeepDF](https://github.com/jesparza/peepdf), aby tworzyć dedykowane skrypty analizy. Ponadto potencjał plików PDF do przechowywania ukrytych danych jest tak duży, że zasoby takie jak przewodnik NSA dotyczący ryzyka i środków zaradczych w plikach PDF, chociaż nie jest już hostowany na swojej pierwotnej lokalizacji, nadal oferuje cenne spostrzeżenia. [Kopia przewodnika](http://www.itsecure.hu/library/file/Biztons%C3%A1gi%20%C3%BAtmutat%C3%B3k/Alkalmaz%C3%A1sok/Hidden%20Data%20and%20Metadata%20in%20Adobe%20PDF%20Files.pdf) oraz zbiór [sztuczek formatu PDF](https://github.com/corkami/docs/blob/master/PDF/PDF.md) autorstwa Ange Albertini mogą zapewnić dodatkową lekturę na ten temat.

<details>

<summary><strong>Naucz się hakować AWS od zera do bohatera z</strong> <a href="https://training.hacktricks.xyz/courses/arte"><strong>htARTE (HackTricks AWS Red Team Expert)</strong></a><strong>!</strong></summary>

Inne sposoby wsparcia HackTricks:

* Jeśli chcesz zobaczyć swoją **firmę reklamowaną w HackTricks** lub **pobrać HackTricks w formacie PDF**, sprawdź [**PLAN SUBSKRYPCYJNY**](https://github.com/sponsors/carlospolop)!
* Kup [**oficjalne gadżety PEASS & HackTricks**](https://peass.creator-spring.com)
* Odkryj [**Rodzinę PEASS**](https://opensea.io/collection/the-peass-family), naszą kolekcję ekskluzywnych [**NFT**](https://opensea.io/collection/the-peass-family)
* **Dołącz do** 💬 [**grupy Discord**](https://discord.gg/hRep4RUj7f) lub [**grupy telegramowej**](https://t.me/peass) lub **śledź** nas na **Twitterze** 🐦 [**@hacktricks\_live**](https://twitter.com/hacktricks\_live)**.**
* **Podziel się swoimi sztuczkami hakerskimi, przesyłając PR-y do** [**HackTricks**](https://github.com/carlospolop/hacktricks) i [**HackTricks Cloud**](https://github.com/carlospolop/hacktricks-cloud) repozytoriów na GitHubie.

</details>