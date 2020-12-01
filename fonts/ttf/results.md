## Fontbakery report

Fontbakery version: 0.7.33

<details>
<summary><b>[1] Family checks</b></summary>
<details>
<summary>⚠ <b>WARN:</b> Is the command `ftxvalidator` (Apple Font Tool Suite) available?</summary>

* [com.google.fonts/check/ftxvalidator_is_available](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/ftxvalidator_is_available)
<pre>--- Rationale ---

There&#x27;s no reasonable (and legal) way to run the command `ftxvalidator` of the
Apple Font Tool Suite on a non-macOS machine. I.e. on GNU+Linux or Windows etc.

If Font Bakery is not running on an OSX machine, the machine running Font
Bakery could access `ftxvalidator` on OSX, e.g. via ssh or a remote procedure
call (rpc).

There&#x27;s an ssh example implementation at:
https://github.com/googlefonts/fontbakery/blob/master/prebuilt/workarounds
/ftxvalidator/ssh-implementation/ftxvalidator


</pre>

* ⚠ **WARN** Could not find ftxvalidator.

</details>
<br>
</details>
<details>
<summary><b>[7] Chokokutai-Regular.ttf</b></summary>
<details>
<summary>🔥 <b>FAIL:</b> Check name table: FONT_FAMILY_NAME entries.</summary>

* [com.google.fonts/check/name/familyname](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/name/familyname)
<pre>--- Rationale ---

Checks that the family name infered from the font filename matches the string
at nameID 1 (NAMEID_FONT_FAMILY_NAME) if it conforms to RIBBI and otherwise
checks that nameID 1 is the family name + the style name.


</pre>

* 🔥 **FAIL** Entry [FONT_FAMILY_NAME(1):WINDOWS(3)] on the "name" table: Expected "Chokokutai" but got "彫刻体". [code: mismatch]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---

Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will
only differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.

However, a quotedbl should have 2 contours, unless the font belongs to a
display family.

This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.


</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: asterisk	Contours detected: 5	Expected: 1 or 4
Glyph name: N	Contours detected: 2	Expected: 1
Glyph name: a	Contours detected: 1	Expected: 2
Glyph name: x	Contours detected: 3	Expected: 1
Glyph name: y	Contours detected: 2	Expected: 1
Glyph name: ordfeminine	Contours detected: 1	Expected: 2 or 3
Glyph name: uni00AD	Contours detected: 0	Expected: 1
Glyph name: Ntilde	Contours detected: 3	Expected: 2
Glyph name: agrave	Contours detected: 2	Expected: 3
Glyph name: aacute	Contours detected: 2	Expected: 3
Glyph name: acircumflex	Contours detected: 2	Expected: 3
Glyph name: atilde	Contours detected: 2	Expected: 3
Glyph name: adieresis	Contours detected: 3	Expected: 4
Glyph name: aring	Contours detected: 3	Expected: 4
Glyph name: ae	Contours detected: 2	Expected: 3
Glyph name: yacute	Contours detected: 3	Expected: 2
Glyph name: ydieresis	Contours detected: 4	Expected: 3
Glyph name: amacron	Contours detected: 2	Expected: 3
Glyph name: abreve	Contours detected: 2	Expected: 3
Glyph name: aogonek	Contours detected: 1	Expected: 2
Glyph name: Nacute	Contours detected: 3	Expected: 2
Glyph name: uni0145	Contours detected: 3	Expected: 2
Glyph name: Ncaron	Contours detected: 3	Expected: 2
Glyph name: Eng	Contours detected: 2	Expected: 1
Glyph name: ycircumflex	Contours detected: 3	Expected: 2
Glyph name: uni01CA	Contours detected: 3	Expected: 2
Glyph name: uni01CB	Contours detected: 4	Expected: 3
Glyph name: aeacute	Contours detected: 3	Expected: 4
Glyph name: uni0201	Contours detected: 3	Expected: 4
Glyph name: uni0203	Contours detected: 2	Expected: 3
Glyph name: uni021B	Contours detected: 1	Expected: 2
Glyph name: uni0233	Contours detected: 3	Expected: 2
Glyph name: uni1EA1	Contours detected: 2	Expected: 3
Glyph name: uni1EA3	Contours detected: 2	Expected: 3
Glyph name: uni1EA5	Contours detected: 3	Expected: 4
Glyph name: uni1EA7	Contours detected: 3	Expected: 4
Glyph name: uni1EA9	Contours detected: 3	Expected: 4
Glyph name: uni1EAB	Contours detected: 3	Expected: 4
Glyph name: uni1EAD	Contours detected: 3	Expected: 4
Glyph name: uni1EAF	Contours detected: 3	Expected: 4
Glyph name: uni1EB1	Contours detected: 3	Expected: 4
Glyph name: uni1EB3	Contours detected: 3	Expected: 4
Glyph name: uni1EB4	Contours detected: 3	Expected: 4
Glyph name: uni1EB5	Contours detected: 2	Expected: 4
Glyph name: uni1EB7	Contours detected: 3	Expected: 4
Glyph name: ygrave	Contours detected: 3	Expected: 2
Glyph name: uni1EF5	Contours detected: 3	Expected: 2
Glyph name: uni1EF7	Contours detected: 3	Expected: 2
Glyph name: uni1EF9	Contours detected: 3	Expected: 2
Glyph name: uni20A6	Contours detected: 2	Expected: 1, 3 or 5
Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7
Glyph name: uni20AD	Contours detected: 2	Expected: 1
Glyph name: uni2116	Contours detected: 5	Expected: 3 or 4
Glyph name: Eng	Contours detected: 2	Expected: 1
Glyph name: N	Contours detected: 2	Expected: 1
Glyph name: Nacute	Contours detected: 3	Expected: 2
Glyph name: Ncaron	Contours detected: 3	Expected: 2
Glyph name: Ntilde	Contours detected: 3	Expected: 2
Glyph name: a	Contours detected: 1	Expected: 2
Glyph name: aacute	Contours detected: 2	Expected: 3
Glyph name: abreve	Contours detected: 2	Expected: 3
Glyph name: acircumflex	Contours detected: 2	Expected: 3
Glyph name: adieresis	Contours detected: 3	Expected: 4
Glyph name: ae	Contours detected: 2	Expected: 3
Glyph name: aeacute	Contours detected: 3	Expected: 4
Glyph name: agrave	Contours detected: 2	Expected: 3
Glyph name: amacron	Contours detected: 2	Expected: 3
Glyph name: aogonek	Contours detected: 1	Expected: 2
Glyph name: aring	Contours detected: 3	Expected: 4
Glyph name: asterisk	Contours detected: 5	Expected: 1 or 4
Glyph name: atilde	Contours detected: 2	Expected: 3
Glyph name: fi	Contours detected: 1	Expected: 3
Glyph name: ordfeminine	Contours detected: 1	Expected: 2 or 3
Glyph name: uni00AD	Contours detected: 0	Expected: 1
Glyph name: uni0145	Contours detected: 3	Expected: 2
Glyph name: uni01CA	Contours detected: 3	Expected: 2
Glyph name: uni01CB	Contours detected: 4	Expected: 3
Glyph name: uni021B	Contours detected: 1	Expected: 2
Glyph name: uni0233	Contours detected: 3	Expected: 2
Glyph name: uni1EA1	Contours detected: 2	Expected: 3
Glyph name: uni1EA3	Contours detected: 2	Expected: 3
Glyph name: uni1EA5	Contours detected: 3	Expected: 4
Glyph name: uni1EA7	Contours detected: 3	Expected: 4
Glyph name: uni1EA9	Contours detected: 3	Expected: 4
Glyph name: uni1EAB	Contours detected: 3	Expected: 4
Glyph name: uni1EAD	Contours detected: 3	Expected: 4
Glyph name: uni1EAF	Contours detected: 3	Expected: 4
Glyph name: uni1EB1	Contours detected: 3	Expected: 4
Glyph name: uni1EB3	Contours detected: 3	Expected: 4
Glyph name: uni1EB4	Contours detected: 3	Expected: 4
Glyph name: uni1EB5	Contours detected: 2	Expected: 4
Glyph name: uni1EB7	Contours detected: 3	Expected: 4
Glyph name: uni1EF5	Contours detected: 3	Expected: 2
Glyph name: uni1EF7	Contours detected: 3	Expected: 2
Glyph name: uni1EF9	Contours detected: 3	Expected: 2
Glyph name: uni20A6	Contours detected: 2	Expected: 1, 3 or 5
Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7
Glyph name: uni20AD	Contours detected: 2	Expected: 1
Glyph name: uni2116	Contours detected: 5	Expected: 3 or 4
Glyph name: x	Contours detected: 3	Expected: 1
Glyph name: y	Contours detected: 2	Expected: 1
Glyph name: yacute	Contours detected: 3	Expected: 2
Glyph name: ycircumflex	Contours detected: 3	Expected: 2
Glyph name: ydieresis	Contours detected: 4	Expected: 3
Glyph name: ygrave	Contours detected: 3	Expected: 2 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are there caret positions declared for every ligature?</summary>

* [com.google.fonts/check/ligature_carets](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/ligature_carets)
<pre>--- Rationale ---

All ligatures in a font must have corresponding caret (text cursor) positions
defined in the GDEF table, otherwhise, users may experience issues with caret
rendering.

If using GlyphsApp, ligature carets can be set directly on canvas by accessing
the `Glyph -&gt; Set Anchors` menu option or by pressing the `Cmd+U` keyboard
shortcut.

If designing with UFOs, (as of Oct 2020) ligature carets are not yet compiled
by ufo2ft, and therefore will not build via FontMake. See
googlefonts/ufo2ft/issues/329


</pre>

* ⚠ **WARN** This font lacks caret position values for ligature glyphs on its GDEF table. [code: lacks-caret-pos]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---

Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).


</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do any segments have colinear vectors?</summary>

* [com.google.fonts/check/outline_colinear_vectors](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_colinear_vectors)
<pre>--- Rationale ---

This test looks for consecutive line segments which have the same angle. This
normally happens if an outline point has been added by accident.

This test is not run for variable fonts, as they may legitimately have colinear
vectors.


</pre>

* ⚠ **WARN** The following glyphs have colinear vectors:
	* uni2606: L<<206.0,478.0>--<370.0,342.0>> -> L<<370.0,342.0>--<388.0,327.0>>
	* uni2606: L<<318.0,111.0>--<479.0,229.0>> -> L<<479.0,229.0>--<500.0,244.0>>
	* uni2606: L<<388.0,327.0>--<381.0,304.0>> -> L<<381.0,304.0>--<318.0,111.0>>
	* uni2606: L<<431.0,459.0>--<403.0,462.0>> -> L<<403.0,462.0>--<206.0,478.0>>
	* uni2606: L<<500.0,244.0>--<521.0,229.0>> -> L<<521.0,229.0>--<682.0,111.0>>
	* uni2606: L<<500.0,672.0>--<440.0,486.0>> -> L<<440.0,486.0>--<431.0,459.0>>
	* uni2606: L<<569.0,459.0>--<560.0,486.0>> -> L<<560.0,486.0>--<500.0,672.0>>
	* uni2606: L<<612.0,327.0>--<630.0,342.0>> -> L<<630.0,342.0>--<794.0,478.0>>
	* uni2606: L<<682.0,111.0>--<619.0,304.0>> -> L<<619.0,304.0>--<612.0,327.0>>
	* uni2606: L<<794.0,478.0>--<597.0,462.0>> -> L<<597.0,462.0>--<569.0,459.0>> and 3 more. [code: found-colinear-vectors]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments?</summary>

* [com.google.fonts/check/outline_jaggy_segments](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments)
<pre>--- Rationale ---

This test heuristically detects outline segments which form a particularly
small angle, indicative of an outline error. This may cause false positives in
cases such as extreme ink traps, so should be regarded as advisory and backed
up by manual inspection.


</pre>

* ⚠ **WARN** The following glyphs have jaggy segments:
	* colonmonetary: L<<273.0,723.0>--<273.0,269.0>>/L<<273.0,269.0>--<380.0,723.0>> = 13.261620741453857
	* f_f_i: L<<382.0,486.0>--<311.0,767.0>>/L<<311.0,767.0>--<311.0,486.0>> = 14.18008194277089
	* perthousand: L<<635.0,723.0>--<356.0,-39.0>>/L<<356.0,-39.0>--<442.0,723.0>> = 13.670581722245533
	* radical: L<<75.0,-12.0>--<-30.0,-175.0>>/L<<-30.0,-175.0>--<71.0,108.0>> = 13.147494021382018
	* uni20AD: L<<309.0,385.0>--<269.0,241.0>>/L<<269.0,241.0>--<346.0,388.0>> = 12.121864366984404
	* uni3043.vert: B<<567.0,305.0>-<590.0,316.0>-<595.0,322.0>>/L<<595.0,322.0>--<407.0,26.0>> = 7.384506329758167
	* uni3043: B<<475.0,219.0>-<498.0,230.0>-<503.0,236.0>>/L<<503.0,236.0>--<315.0,-60.0>> = 7.384506329758167
	* uni3083.vert: L<<510.0,299.0>--<510.0,-26.0>>/L<<510.0,-26.0>--<395.0,454.0>> = 13.47315811273114
	* uni3083: L<<432.0,234.0>--<432.0,-91.0>>/L<<432.0,-91.0>--<317.0,389.0>> = 13.47315811273114
	* uni30C3.vert: L<<975.0,738.0>--<539.0,-24.0>>/L<<539.0,-24.0>--<758.0,738.0>> = 13.742526575121833 and 4 more. [code: found-jaggy-segments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines?</summary>

* [com.google.fonts/check/outline_semi_vertical](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical)
<pre>--- Rationale ---

This test detects line segments which are nearly, but not quite, exactly
horizontal or vertical. Sometimes such lines are created by design, but often
they are indicative of a design error.

This test is disabled for italic styles, which often contain nearly-upright
lines.


</pre>

* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:
	* C: L<<688.0,800.0>--<689.0,546.0>>
	* Ccedilla: L<<688.0,800.0>--<689.0,546.0>>
	* E: L<<589.0,229.0>--<590.0,-24.0>>
	* E: L<<590.0,800.0>--<589.0,546.0>>
	* Ebreve: L<<43.0,773.0>--<550.0,774.0>>
	* Ebreve: L<<589.0,228.0>--<590.0,-25.0>>
	* Ebreve: L<<590.0,800.0>--<589.0,545.0>>
	* Ecaron: L<<43.0,773.0>--<550.0,774.0>>
	* Edieresis: L<<590.0,229.0>--<591.0,-24.0>>
	* Edieresis: L<<591.0,800.0>--<590.0,546.0>> and 212 more. [code: found-semi-vertical]

</details>
<br>
</details>

### Summary

| 💔 ERROR | 🔥 FAIL | ⚠ WARN | 💤 SKIP | ℹ INFO | 🍞 PASS | 🔎 DEBUG |
|:-----:|:----:|:----:|:----:|:----:|:----:|:----:|
| 0 | 1 | 7 | 91 | 7 | 88 | 0 |
| 0% | 1% | 4% | 47% | 4% | 45% | 0% |

**Note:** The following loglevels were omitted in this report:
* **SKIP**
* **INFO**
* **PASS**
* **DEBUG**
