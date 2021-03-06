# Bachelor's Thesis
### Static Analysis Using Facebook Infer to Find Atomicity Violations

---

# Bakalářská práce
### Statická analýza v nástroji Facebook Infer zaměřená na detekci porušení atomičnosti

---

##### Author: Dominik Harmim <xharmi00@stud.fit.vutbr.cz>

##### Supervisor: [prof. Ing. Tomáš Vojnar, Ph.D.](http://www.fit.vutbr.cz/~vojnar) (UITS FIT VUT) <vojnar@fit.vutbr.cz>

##### Reviewer: [Ing. Aleš Smrčka, Ph.D.](http://www.fit.vutbr.cz/~smrcka) (UITS FIT VUT) <smrcka@fit.vutbr.cz>

##### Specification:
1. Prostudujte principy statické analýzy založené na abstraktní interpretaci.
   Zvláštní pozornost věnujte přístupům zaměřeným na odhalování problémů v
   synchronizaci paralelních procesů.
2. Seznamte se s nástrojem Facebook Infer, jeho podporou pro abstraktní
   interpretaci a s existujícímí analyzátory vytvořenými v prostředí Faceboook
   Infer.
3. V prostředí Facebook Infer navrhněte a naimplementujte analyzátor zaměřený
   na odhalování chyb typu porušení atomicity.
4. Experimentálně ověřte funkčnost vytvořeného analyzátoru na vhodně zvolených
   netriviálních programech.
5. Shrňte dosažené výsledky a diskutujte možnosti jejich dalšího rozvoje
   v budoucnu.

##### Category: Software analysis and testing

##### Implementation language: [OCaml](https://ocaml.org)

##### Free software: [Facebook Infer](https://fbinfer.com)

##### Literature:
- Nielson, F., Nielson, H.R., Hankin, C.: Principles of Program Analysis,
  Springer-Verlag, 2005.
- Blackshear, S., O'Hearn, P.: Open-Sourcing RacerD: Fast Static Race Detection
  at Scale, 2017. Dostupné on-line:
  https://code.fb.com/android/open-sourcing-racerd-fast-static-race-detection-at-scale.
- Atkey, R., Sannella, D.: ThreadSafe: Static Analysis for Java Concurrency,
  Electronic Communications of the EASST, 72, 2015. Dostupné on-line:
  https://bentnib.org/threadsafe.html.
- Bielik, P., Raychev, V., Vechev, M.T.: Scalable Race Detection for
  Android Applications, In: Proc. of OOPSLA'15, ACM, 2015.
- Dias, R.J., Ferreira, C., Fiedor, J., Lourenço, J.M., Smrčka, A., Sousa, D.G.,
  Vojnar, T.: Verifying Concurrent Programs Using Contracts, In: Proc. of
  ICST'17, IEEE, 2017.

## Implementation
The implementation is in the repository
[harmim/infer](https://github.com/harmim/infer). It is a fork of the repository
[facebook/infer](https://github.com/facebook/infer). It is implemented under
the branch [atomicity-sets](https://github.com/harmim/infer/tree/atomicity-sets),
see the [diff](https://github.com/facebook/infer/compare/master...harmim:atomicity-sets).

## Wiki
More information about the product, including examples, installation, and usage
are available at the [Wiki](https://github.com/harmim/infer/wiki/Atomer:-Atomicity-Violations-Analyser).

## Useful links:
- [Facebook Infer](https://fbinfer.com)
- [Facebook Infer GitHub](https://github.com/facebook/infer)
- [OCaml](https://ocaml.org)
- [Real Wolrd OCaml](https://v1.realworldocaml.org/v1/en/html/index.html)
- [Abstract interpretation - Patrick Cousot intro](https://www.di.ens.fr/~cousot/AI/IntroAbsInt.html)
- [Facebook Infer lab](https://github.com/facebook/infer/tree/master/infer/src/labs)
- [Facebook Infer presentation](https://fbinfer.com/downloads/pldi17-infer-ai-tutorial.pdf)
- [Facebook Infer INSTALL](https://github.com/facebook/infer/blob/master/INSTALL.md)
- [Facebook Infer CONTRIBUTING](https://github.com/facebook/infer/blob/master/CONTRIBUTING.md)
- [Open-sourcing RacerD: Fast static race detection at scale](https://code.fb.com/android/open-sourcing-racerd-fast-static-race-detection-at-scale)
- [ThreadSafe: Static Analysis for Java Concurrency](https://bentnib.org/threadsafe.html)
- [Scalable Race Detection for Android Applications](https://dl.acm.org/citation.cfm?id=2814303)
- [Verifying Concurrent Programs Using Contracts](https://ieeexplore.ieee.org/document/7927975)
- [How to Use C Mutex Lock](https://www.thegeekstuff.com/2012/05/c-mutex-examples)
- [A True Positives Theorem for a Static Race Detector](https://arxiv.org/abs/1811.03503)
- [Gluon](https://github.com/trxsys/gluon)
- [VeriFIT Static Analysis Plugins](http://www.fit.vutbr.cz/research/groups/verifit/tools/sa-plugins)
