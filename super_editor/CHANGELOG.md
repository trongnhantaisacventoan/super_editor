## [0.2.3-dev.1] - Nov 11, 2022: SuperReader, Bug Fixes (pre-release)
 * The same as v0.2.3+1, but compatible with Flutter `master`

## [0.2.3+1] - Nov, 2022: Pub.dev listing updates
 * No functional changes

## [0.2.3] - Nov, 2022: SuperReader, Bug Fixes
 * FEATURE: SuperReader - Created a `SuperReader` for read-only documents (0424ff1c6695629d2dba8214a950d261a3002b02)
 * FEATURE: SuperEditor - Simulate IME text input for tests (3b67328722288d9c31ac52bed1bce4a550868e58)
 * FEATURE: SuperEditor - linkify pasted text (397e373c3f53844b7b7e644c6dccbe7a7c02b822)
 * FEATURE: SuperTextField - Add padding property (2437d84735556cd4aaa30c61f413eefe7c51bbcb)
 * FEATURE: SuperEditor - Align text with stylesheet rules (23fb39aa0aecdd611106f5d7d75bbfbeb0e0ce5a)
 * FIX: SuperEditor - scrolling a document that sits in a horizontal list view (f8aec2e84782f4976f26e14880770611337b8e82)
 * FIX: SuperTextField - scrolling behavior when `maxLines` is `null` (f31fe207538aea76ef78242810ff85850b4cda63)
 * FIX: SuperEditor - scroll jumping when typing near the top/bottom editor boundary (c2485223059f84f52a7cdb5de62a7a9ca00fe32c)
 * FIX: SuperTextField - horizontal alignment (6704f8e1ab4c6e4fdf46e73daf6e5f58b897e23f)
 * FIX: SuperTextField - Remove focus when detached from IME on iOS (5f0d921d885068da408359def576b021ba6aa151)
 * FIX: SuperTextField - Hint text cut off on desktop (d1214e97d0c255b9ab2c5cb6d9b3ead40aced0c9)
 * FIX: SuperEditor - set selection when editor receives focus (c866122e52b22c995630d673c2af8258722e04ec)
 * FIX: SuperEditor - Caret display when editor receives focus (ecc0af2e4380be9d8250f51f1f75fbdb780a3432)
 * FIX: SuperTextField - Exception during hot reload on desktop (4ae59142ae4c7e5e2e151683ff7bc941505b366f)
 * FIX: SuperTextField - Bad line height estimation on Mac (16fa1e993907bf06cd10abca853ddcb57d46212d)
 * FIX: SuperEditor - Ignore pointer events on block quote so selection works (700f0f752f9b0ac2ee05ea10e79edf97f114c26c)
 * FIX: SuperEditor - Serialization and deserialization of empty paragraphs (1601fdce95ebfa34bddf80cab3e58e700b0edec3)
 * FIX: SuperEditor - Caret placement when indenting a list item (595a5704f4ebabfb0a90ee2568591af28ecbf96c)
 * FIX: SuperEditor - Trackpad scrolling due to Flutter change (f4d342c161432f3ccf94c72d251f72eb1ae58754)
 * FIX: SuperEditor - Image scrolling with mouse wheel (874df02ad2759a0c2615e4f3521bda3d6e261c31)
 * FIX: SuperEditor - List indentation using TAB key (f1570ec515218cd525c4c7e5d41d39373ccab210)
 * FIX: SuperEditor - Selection when tapping beyond end of document (d5e7460956fc6d60abd65991d48ca2c073c1da38)
 * FIX: SuperEditor - Crash when changing gesture mode (b9f868766767756ad589984d74089ef780809b95)
 * FIX: SuperEditor - Respect `TextAffinity` for selection (0c50b67f5ef4e0e8d4ee0fc9a7e625d84c5027db)
 * FIX: SuperEditor - Default gesture mode (63bb2f283efd4e773bd86651709bdc11d1614547)
 * FIX: SuperEditor - List item style when converting to paragraph and back again (7db7fcd84e8fc3715448eda6d7ec9cc754c29f0b)
 * FIX: SuperTextField - Viewport height when text changes on mobile (376c0b6856f217b7364ee81cad41140f7132a570)
 * FIX: SuperEditor - Desktop scroll momentum that was broken by Flutter 3.3.3 (f7f20b93cb0d86246f501e20d871806df6140b5d)
 * FIX: SuperEditor - Floating cursor opacity (dec4bd3076efffe5f795bf88f8d7dbffbe94732f)
 * FIX: SuperEditor - Typing lag in large documents (ae571decde5884fd246f858754dfc71b4e4fabc5)


## [0.2.2] - July, 2022: Desktop IME
 * Use the input method engine (IME) on Desktop (previously only available on mobile)
 * A number of `SuperTextField` fixes and improvements. These changes are part of the path to the next release, which is focused on stabilizing `SuperTextField`.

## [0.2.1] - ~July, 2022: Desktop IME~ (Removed from pub)
 * Use the input method engine (IME) on Desktop (previously only available on mobile)
 * A number of `SuperTextField` fixes and improvements. These changes are part of the path to the next release, which is focused on stabilizing `SuperTextField`.

## [0.2.0] - Feb, 2022: Mobile Support
 * Mobile document editing
 * Mobile text field editing
 * More document style controls

## [0.1.0] - June 3, 2021

The first release of Super Editor.

 * Document and editor abstractions
   * See `Document` for a readable document
   * See `MutableDocument` for a mutable document
   * See `DocumentEditor` to commit document changes in a transactional manner
   * See `DocumentSelection` for a logical representation of selected document content
   * See `DocumentLayout` for the base abstraction for a visual document layout
 * Out-of-the-box editor: Commonly used types of content, visual layout, and user interactions are supported
   by artifacts available in the `default_editor` package.
 * Markdown serialization is available in the `serialization` package.
 * SuperTextField: An early version of a custom text field called `SuperTextField` is available in
   the `infrastructure` package.
 * SuperSelectableText: All text display in Super Editor is based on the `SuperSelectableText` widget,
   which is available in the `infrastructure` package.
 * AttributedText: a logical representation of text with attributed spans is available
   in the `infrastructure` package.
 * AttributedSpans: a logical representation of attributed spans is available in the
   `infrastructure` package.
