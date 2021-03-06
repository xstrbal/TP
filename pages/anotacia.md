Na dôležitosť tejto témy upozornil aj americký inštitút pre štandardy a technológiu NIST v správe Report on Post-Quantum Cryptography (správa je dostupná na [NIST.IR.8105](https://nvlpubs.nist.gov/nistpubs/ir/2016/NIST.IR.8105.pdf)). NIST zároveň vyhlásil súťaž [Post-Quantum Cryptography Standardization Process](https://csrc.nist.gov/Projects/Post-Quantum-Cryptography/Post-Quantum-Cryptography-Standardization) s cieľom navrhnúť nové kryptografické štandardy odolné voči kvantovým počítačom. Do súťaže prišlo vyše 60 návrhov kryptosystémov (všetky návrhy su verejne dostupné na [Nist](https://csrc.nist.gov/projects/post-quantum-cryptography/round-1-submissions)). Tieto návrhy budú v najbližších rokoch verejne analyzované vedeckou komunitou s cieľom vybrať najlepších kandidátov.

Viacero návrhov zaslaných do súťaže je založených na QC-LDPC McElieceovom kryptosystéme. Jedná sa o variant McElieceovho kryptosystému, v ktorom sa využívajú QC-LDPC kódy. Pri šifrovaní sa správa prevedie na kódové slovo QC-LDPC kódu a ku kódovému slovu sa pridá chyba. Pri dešifrovaní je potrebné túto chybu odstrániť. Chybu je možné odstrániť použitím tajného kľúča, ktorý obsahuje matice H a Q. Na odstránenie chyby je možné použiť dve metódy: buď sa použije dekódovací algoritmus pre QC-LDPC kódy, ktorý využíva maticu H, alebo sa použije dekódovací algoritmus pre QC-MDPC kódy, ktorý používa maticu H*Q. Cieľom práce je porovnať efektívnosť týchto dvoch metód.

## Úlohy:

+ Naštudujte princípy fungovania QC-LDPC McElieceovho kryptosystému.

+ Oboznámte sa s implementáciou QC-LDPC McElieceovho kryptosystému v knižnici BitPunch (implementácia je v jazyku C).

+ Porovnajte efektívnosť dvoch vyššie spomenutých metód na odstránenie chyby zo správy zašifrovanej QC-LDPC McElieceovym kryptosystémom.
