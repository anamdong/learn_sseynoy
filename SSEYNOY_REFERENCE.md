# Sseynoy (胡語): descriptive grammar and linguistic reference

**Current specification — 21 November 2026 (2026-11-21).** This is the current Codex handoff for the constructed Sinitic language Sseynoy. It incorporates the creator's phonetic annotations and grammatical responses after the earlier 19 November dossier. The earlier report is preserved in `legacy/REFERENCE-2026-11-19.md` for historical character-reading surveys and source history, not as the current grammar. Read `AGENTS.md` before generating language data.


### Release changes — 2026-11-21

**Authoritative pronoun reform:** previous `tsòi` → `soi` (I/me, /soj/, level); `zzhi` → `je` (you, /dʑe/, level); genitives `tsèk` → `sek` and `zzhek` → `jek`. New plural `soidáy`, `jedáy`; new plural genitives `soidáydek`, `jedáydek`. The third-person system `y`, `ydáy`, `ydek`, `ydáydek` is unchanged. The historical spellings remain in `legacy/`; they are **not current standard Sseynoy**. Case and capitalization vary by sentence position.

**Pronunciation expansion:** `oi`=/oj/, `oy`=/oy/, `ai`=/aj/, `ei`=/ej/, `ui`=/uj/, `aei`=/ɛj/, `aey`=/ɛy/, `uei`=/yj/, `ey`=/iː/ (not a diphthong). `au` and `aw` both represent /au/. Creator confirms phonemic distinction of `oi` and `oy` in all environments, and single diphthong phoneme analysis. Newly confirmed reading: 鞋 `haey`, 害 `hàei`. See `data/diphthongs.tsv` and `data/character_reading_overrides_2026-11-21.tsv`.

The examples in `data/examples.tsv` are **modernized editorial adaptations** of earlier creator-authored examples, not newly elicited utterances. Their original values are preserved in `legacy/examples-2026-11-20.tsv` and the `modernized_from_2026_11_20` field. This distinction matters when quoting evidence.

## 1. Evidence and typological overview

Sseynoy is predominantly analytic, with SVO basic order, prenominal possessors and relative clauses, lexical tone, classifiers, and limited nominal suffixation and irregular pronominal inflection. Colloquial usage employs native vocabulary and grammatical forms; Sino-derived vocabulary is especially characteristic of formal/literary usage. The distinction is clearest in pronouns. Native etymologies range from potentially irregular Sinitic forms to uncertain origins; no imagined pre-Sinitic ancestry is established. Native roots are mostly monosyllabic, not necessarily exclusively so. Mixed native/Sino-derived compounds are generally permitted. No obligatory verbal agreement, gender, or tense conjugation is demonstrated, but absence is not yet proven.

Evidence priority: explicit creator corrections > creator-authored examples > batch acceptance of assistant proposals > inherited character data for the relevant stratum > hypotheses. See `legacy/examples-2026-11-20.tsv` for verbatim original examples and `data/examples.tsv` for modernized versions with provenance and `data/acceptability.tsv` for rejected or dispreferred forms. Batch acceptance means the construction was accepted generally, not that each character spelling was checked. Do not replace spellings from the source examples in silence. Historical reconstructions, assigned Hanzi for native morphemes, and analyses of grammaticalization are not settled.

## 2. Phonology and orthography (音韻・正書法)

### 2.1 Vowels

The creator's handwritten charts (copies in `corpus/IMG_0306.jpeg`–`IMG_0308.jpeg`) and later answers specify these values. IPA is a transcription of the annotations; phonemic contrast must be independently established for all sound pairs. Ten basic monophthong qualities are attested: /a ɛ e ɔ œ i ɪ o u y/.

| Spelling | IPA | Spelling | IPA |
|---|---|---|---|
| a | a | aa, ah | aː |
| ae | ɛ | e | e |
| eo | ɔ | oe | œ |
| i | i | y (nucleus) | ɪ |
| o | o | u | u |
| ue | y | ey | iː |
| ueh | yː | eomh | ɔːm |
| emh | eːm | ann | ã ~ ãː |

All monophthong qualities can be nasalized. Whether every oral/nasal and length combination has lexical minimal pairs remains open. The spelling ann admits both lengths. Here h can indicate vowel length, including before final m even when written after m; do not apply a universal h rule until all contexts are checked. aa and ah are homophonous.

| Spelling | IPA | Example | Notes |
|---|---|---|---|
| oi | /oj/ | soi | a single diphthong; /j/ offglide |
| oy | /oy/ | coy | a single diphthong; front-rounded /y/ offglide |
| ai | /aj/ | bài | confirmed |
| ay | /ay/ | lay | distinct from ai |
| ei | /ej/ | sùei | in uei; see parsing below |
| ui | /uj/ | kuín | confirmed |
| uy | /uy/ | guy | distinct from ui |
| au, aw | /au/ | diáu; gaw | alternative spellings, same phonetic value |
| aei | /ɛj/ | hàei 害 | falling tone; near-minimal contrast with 鞋 |
| aey | /ɛy/ | haey 鞋 | level tone; near-minimal contrast with 害 |
| aew | /ɛu/ | haew | confirmed |
| iw | /iu/ | gíw | confirmed |
| ou | /ou/ | ou | confirmed |
| eu | /eu/ | eu | confirmed |
| uei | /yj/ | sùei /syj/ | parse ue as /y/ before final i /j/ |
| aay | /aːy/ | — | long first element; example not specified |
| aaw | /aːu/ | — | long first element; example not specified |
| ey | /iː/ | gwey | **NOT a diphthong**, long monophthong |

The user specifies diphthongs as **single diphthong phonemes**, not two heterosyllabic vowels. In diphthongal offglide position, grapheme `i` corresponds to /j/, while grapheme `y` corresponds to high front rounded /y/. `oi` /oj/ and `oy` /oy/ remain phonemically distinct in all environments; `aei` /ɛj/ and `aey` /ɛy/ are also distinct (although the two cited words differ additionally in tone). Do not treat `ey` as a diphthong.

**Parsing rule:** identify multigraph monophthong spellings (especially `ue`=/y/, `ae`=/ɛ/) before analyzing a final `i` as an offglide /j/. A written `i` preceding the main vocalic nucleus is a medial /j/; following it, it may be an offglide /j/. This is creator-confirmed. Illustrations analyzed as onset + medial + diphthong, **not triphthongs**: `miaw` = m + /j/ + /au/; `miáew` = m + /j/ + /ɛu/; `liou` = l + /j/ + /ou/. These schematic syllabifications are confirmed by the creator; avoid extending them mechanically where morphology or syllable breaks remain unclear.

Initial y = /j/, w = /w/; medial i can be /j/. Distinguish true diphthongs from medial glide + nucleus and digraph monophthongs. Nasalized diphthongs and genuine diphthong + coda sequences remain unverified. Long vowels before unreleased stops are allowed.

### 2.2 Onsets

| Grapheme | Phonetic realization (broad) |
|---|---|
| b | [b ~ ʔp] |
| p | [pʰ] |
| d | [d ~ ʔt] |
| t | [tʰ] |
| g | [ɡ ~ ʔk] |
| k | [kʰ] |
| f | [f] |
| v | [v] |
| m | [m] |
| n | [n] |
| nh | [ɲ] |
| h | [h] |
| j | [dʑ] |
| c | [tsʰ] |
| z | [dz ~ z ~ ʔts] |
| s | [s] |
| x | [ɕ] |
| zh | [dʒ] |
| ch | [tʃʰ] |
| sh, ssh | [ʃ] |
| l, lh | [l] |
| r | [ɹ] (handwritten rhotic transcription to verify) |
| w | [w] |
| y | [j] |

The b/d/g voiced versus preglottalized realizations are individual variation, not conditioned by phonological environment. The small suprasegmental marks and some consonant symbols in the handwritten chart are visually ambiguous; the original image is authoritative. zzh, ss and lh are spelling conventions, not intrinsically distinct phonemes; ssh/sh and lh/l share phonemes as explicitly annotated. Exact mapping for all native doubled spellings remains to be checked; do not infer an IPA value by doubling a consonant. nh is a real palatal nasal and also characteristic of native vocabulary. An onset inventory cannot yet guarantee that each listed phonetic realization is an independent phoneme.

### 2.3 Codas

| Spelling | IPA / description |
|---|---|
| p | [p̚] |
| t | [t̚ ~ ʔ] |
| k | [k̚] |
| v | [v] |
| ts | [ts] |
| ch | [x] |
| n | [n] |
| m | [m] (attested in emh/eomh) |
| ng | nasal coda, usual interpretation [ŋ], not separately elicited |
| nh | palatal nasal [ɲ] |
| nn | vowel nasalization (ann above) |
| r | rhotic consonant, ar transcribed /aɹ/ |

Stop vs continuant/affricate codas are distinct in pronunciation; their correspondence with historical *-p, *-t, *-k is a historical hypothesis. A general working syllable template is (C)(G)V(secondary vowel or glide)(C), with vowel quantity and nasalization and lexical tone. This is not a validated complete phonotactic grammar.

### 2.4 Tone and connected speech

| Mark | Contour | Traditional category (working label) |
|---|---|---|
| unmarked | level, mid to high pitch | 平 |
| acute | rising | 上 |
| grave | falling | 去 |
| checked syllable | similar pitch behavior to unmarked | 入 |

Three pitch contours, with a segmentally distinguished entering-tone class. Exact pitch endpoints and historical category mapping for individual readings are not fully established. No obligatory consecutive-rising-tone sandhi. Optional reduction of the first rise was discussed but never adopted. Unstressed grammatical particles may undergo tonal reduction (creator's tentative “tone lenition”). Resyllabification across a consonant-final / vowel-initial boundary occurs; exact release, voicing and domain rules unknown. Do not write new tone marks as a result of connected-speech hypotheses.

### 2.5 Writing and lexical strata

Character readings are primarily monosyllabic; most lexical words may comprise one or multiple such morphemes. The Latin script has nonphonemic conventions that can distinguish native forms and historical spellings; reverse IPA lookup is not uniquely reversible. Retain acute/grave marks, apostrophes, hyphens, and known concatenation. Examples: gweyga, zaakrit, myngrit; numeral-classifier it-gàa, it-gueon; contracted zhi'ng, oe'ng, shik'gwa; plural soidáy; use original spelling sik in the attested relative clause rather than silently correcting it. Capitalization varies in sources. Native (純胡文) vs Sino-derived readings are not interchangeable in every context. The inherited dictionary preferred column may be Sino-derived even where colloquial forms are explicitly known (e.g. 我 áa vs **soi**; 汝 rúe vs **je**; 胡 hou vs ssey; 語 úh vs nòy). Do not replace one with the other in the base data. Source: earlier dictionary report; see `data/native_readings_reported.tsv` for reported native entries, separate from explicit evidence. Former `tsòi/zzhi` in the inherited dictionary or quoted corpus are **historical** and not a reason to revert the reform.

## 3. Nominal structure (名詞句)

### 3.1 Pronouns

| Person | Singular | Plural | Singular genitive | Plural genitive |
|---|---|---|---|---|
| 1 | soi | soidáy | sek | soidáydek |
| 2 | je | jedáy | jek | jedáydek |
| 3 | y | ydáy | ydek | ydáydek |

The singular first and second possessives are **confirmed contracted forms** (sek, jek), following the creator’s 2026-11-21 reform, while plural forms permit pronoun + -dáy + -dek. Third person y is attested with both male and female English referents. The same base forms occur in subject, direct object and recipient positions; other cases and inclusive/exclusive distinctions untested. gy is used in a possessive relative (its/her father), not assumed a colloquial synonym in every context. See exact paradigm `data/pronouns.tsv`.

### 3.2 Number, classifiers and determination

-dáy is accepted for pronouns and animate nouns rindáy (people), kuíndáy (dogs); generalization to inanimate nouns is untested. It is not assumed obligatory with plural referents. Numeral + classifier + noun: it-gueon shuh / it-gàa shuh (a book), it-gàa kuín (a dog). gueon is specialized for books in the attested context; gàa general. Bare nouns can be definite or generic. Attested determiners:

| Form | Meaning |
|---|---|
| kuín | the dog / dogs in general |
| it-gàa kuín | a dog |
| gàa kuín | a certain dog |
| sah kuín | some dogs |
| ca kuín | this dog |
| na kuín | that dog |
| biet gàa kuín | another dog |
| máy gàa kuín | every dog |
| rimka kuín | any dog |

Creator tentatively suggests gàa is preferred in contexts using an English indefinite article. It is not established as obligatory; no definite article demonstrated.

### 3.3 Possession

Prenominal inflected pronoun: sek ga, jek fú, ydek shuh. Free pronoun + dek also acceptable: soi dek ga. Nominal possessor + gàa + noun: John gàa ga, kuín gàa coy. Johndek rejected; soi gàa ga sounds a bit off. Independent possessive: Ca shuh vi soi gàa (yeo). Multiple functions of gàa are attested; their etymological relationship is only a hypothesis. Existential possession: Soi yóu it-gueon shuh (yeo). / Soi yóu it-gàa shuh (yeo).

## 4. Clause structure and predicate types (句法)

Basic order SVO: Soi hàw je. (I like you.) Intransitive SV: Fay fà yí. Property predicates need no overt copula: Y gaw. (He is tall.) Nominal identity uses vi: Ca vi sek shuh. Subject may be omitted when recoverable: Myngrit gìn. (See you tomorrow.) Imperative omits subject: Gip soi sah coy. Recipient precedes theme in attested double-object construction. No obligatory person/number inflection is shown. Adjective position outside predicates is inferred, not extensively elicited.

## 5. Tense, aspect and negation (時制・相・否定)

| Form | Function | Exact example |
|---|---|---|
| unmarked | simple predicate | soi zhi. |
| ýzin | anterior temporal reference | soi ýzin zhi shé. |
| oe | progressive | Je oe vi ka keo? |
| shé cheng | in-process construction | Soi oe gweyga shé cheng. |
| yí | postpredicative completion/anteriority | Soi kay moen yí. |
| bet | finish (lexical/resultative) | Soi shik bet shé yí. |
| zung … 'gwa | experiential | soi zung shik'gwa shé. |
| mèy | not yet | soi mèy shik. |
| gé fue zàey | no longer | soi gé fue zàey shik. |
| fut / fue | general preverbal negation (same morpheme per creator) | Soi fue yok xàng |
| 'ng | lexically restricted negative contraction | soi zhi'ng. / soi oe'ng shik. |
| mut | prohibitive | mut shik ca. |

The exact function of clause-final shé in past/experiential examples, and yí as perfective vs perfect vs completive, are provisional. Both oe shik and shik shé cheng were accepted. Negative clitic also occurs on yí in Je shik fàen yí'ng? (Have you eaten yet?). shik'ng and yok'ng explicitly rejected: use fue shik and fue yok. Do not assume the negative contraction productive on all predicates or infer its phonetics. Modal negation precedes modal: soi fue nay (nung) shik ca. No tense conjugation established; time reference can come from adverbs and context.

## 6. Questions and responses (疑問・應答)

Wh-in-situ: Je oe vi ka keo?; Je oe xàng kachúh keo? keo is a question particle; yí'ng also questions completed action. yeo is optional in the identity/possession examples, with exact discourse function still open. Independent ren = yes, bóu = no; predicate echoing also works. Negative-question response alignment not known.

## 7. Relative clauses (關係節)

Head-final attributive phrase: relative clause + shé + head. Subject gap lacks só in attested examples; non-subject object and location relatives have só before the predicate. Possessive relative has resumptive-like gy. Examples:

| Type | Exact phrase |
|---|---|
| Subject | Hàw soi shé rin |
| Object, past | Soi zaakrit só gìn shé kuín |
| Object | Je só máay shé shuh |
| Object, progressive | Soi só oe sik shé shikmut |
| Locative | Soi só zhùu shé ga |
| Genitive | Gy fú vi gawshy shé nhúrin. |
| Subject, ditransitive clause | Gip soi ca shuh shé rin. |

Do not infer indirect-object or comparative relativization from these. The last example relativizes the giver, not the recipient. só is the reading associated with 所; shuh is book. Tone matters.

## 8. Space, direction, serial verbs (空間・連動)

oe + noun + spatial term: Shuh oe zhak sàng.; Kuín oe zhak hàe.; Y lip oe sek byeng. Existential locative can precede yóu: Ga hòew yóu it-gàa much. Source zỳ + NP may precede or follow verb: Soi lay zỳ Ritfón. / Soi zỳ Ritfón lay. Directional xàng is used in Soi oe xàng Chengguk. Enter/exit rip/chut: Y bòe rip shit.; Y cú chut shuh zỳ dàay cheng / Y zỳ dàay cheng cú chut shuh. This shows flexible source placement in these specific contexts, not free word order generally. Motion + purpose: Soi xàng máay shikmut. Serial actions with or without yr: Lay yr gìn. / Lay gìn.; Zàang ca shuh yr gweyga. Perception + embedded clause: Soi ting y chànggaa.; Soi gìn y rip ga.

## 9. Resultatives, voice, causation, modality (結果・態・樣態)

Transitive resultative: Soi dáangfà fay yí. Intransitive result: Fay fà yí. Postverbal bet completion: Soi shik bet shé yí. Passive exact construction: Kuín bỳ iaw oe ta kuín. (The dog was bitten by another dog.) Patient + bỳ + verb + oe + agent; agent optionality remains open. ta in this example means other/another in context; do not equate automatically with pronoun y or substitute biet gàa. Accepted causative and permission: Soi shí y shik.; Soi yúng y gweyga. Modals precede verb. nay/nung ability; káa permission; ýng should; su must; huek possibility; yok desire; neng preference (would rather). Exact evidence in examples.tsv. su is not bitxu here; neng not ning.

## 10. Comparison and degree (比較・程度)

| Construction | Exact example |
|---|---|
| positive A + adjective | Y gaw. |
| comparative A + adjective + oe + B | Y gaw oe soi. |
| equative A + yu + B + dueng + adjective | Y yu soi dueng gaw. |
| superlative zùy + adjective | Y zùy gaw. |
| excessive gwà + adjective | Ca gwà gwèy. |
| excessive after verb | Soi shik gwàdaa. |
| insufficient fue zoch + adjective | Ca fue zoch dàe |
| slight degree liak | Soi liak háey. |
| correlative yúu … yúu | Soi yúu duek yúu háey. |
| alternate correlative | Soi duek shé yúu daa, háey yik yúu myng. |

## 11. Complex sentences (複文)

The following proposed constructions received batch acceptance except for specific corrected sentences. Exact spellings still require dictionary/context verification: Rae je lay, soi zuk xàng. (if … then); Rae hàe úe, soi zuk fue xàng. (if it rains); Swi y nien'iù, gach chungmyng. (although); Soi yin by yr fue xàng. (because); Soi ývi y sí. (think); Soi hywang je lay. (hope); Soi zhi y hàw soi. (know); Y vet y by. (say); Soi yok je xàng. (want). Complement clauses follow verbs without an overt complementizer in these examples. Temporal clauses: dáey soi gwey. (wait until I return); Shik zin sý jek shóu (wash your hands before eating); Shik bet hòew, soi gweyga yí. (after eating, I went home; batch accepted). Preference: Soi neng lèou oe cachúh. (rather stay here). Be careful: no invented character readings, even if syntax is hypothetical.

## 12. Lexicon and character system (語彙・漢字音)

`data/dictionary.tsv` preserves the prior 1,253-character snapshot, preferred and earlier variant fields. `data/reading-tests.tsv` contains historical reading diagnostics. `data/homophones.tsv` and `data/variants.tsv` reflect that snapshot only. `data/inferred.tsv` is historical speculation, not authoritative. `data/words.tsv` indexes useful words and grammatical forms from examples by meaning and evidence status; an English gloss does not establish a unique Hanzi mapping or lexical etymology. `data/native_readings_reported.tsv` retains previously reported native mappings; not directly rechecked in this build. Where explicit spelling corrections apply, use the new evidence: sý (wash), shóu (hand), neng (rather), su (must), iaw (bite), dáey (wait), bet (finish), zùy (most). Earlier assistant Hanzi assignments for new words are not authoritative unless found in dictionary or explicitly supplied. Character dictionary is not the same as a bilingual word dictionary.

For original character correspondence surveys (traditional 36 initials, historical open/nasal/checked rimes, numeric/calendrical vocabulary, homophones and variant history), see `legacy/REFERENCE-2026-11-19.md` §§5–9, 11–12 and Appendix A. Those sections predate the confirmed IPA and grammar; treat their phonetic claims as historical hypotheses. The legacy translator and learning application may contain errors or outdated conventions; do not use them as authoritative data.

## 13. Development workflow

Use `AGENTS.md`, this specification, and the TSV data as primary project context. Validate translations against exact attested constructions and lexical forms; bracket genuinely missing readings instead of guessing. Note uncertainty separately. Keep a record of new creator corrections and retain old raw source lines. Do not auto-generate missing pronunciations via Mandarin, Korean, Middle Chinese or analogical sound changes. To continue research, see `QUESTIONS.md`. Source website: https://anamdong.github.io/sseynoydict/ (not freshly retrieved in this build). The packaged data and annotation images are offline evidence; they do not guarantee synchronization with the live dictionary.
