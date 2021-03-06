# Report Customizer for Zotero

Install by downloading the [latest version](https://github.com/retorquere/zotero-report-customizer/releases), and then

1. In the main menu go to Tools > Add-ons
2. Select 'Extensions'
3. Click on the gear in the top-right corner and choose 'Install Add-on From File...'
4. Choose .xpi that you've just downloaded, click 'Install'
5. Restart Zotero

Does what [Jason Priem's "Report Cleaner"](http://jasonpriem.org/projects/report_cleaner.php), but
without the copy-paste-into-website bit. You can live-edit the report to pick the elements to remove
from the report, and they will simple not show up from that point on.

## Integration with [Zotero: Better BibTeX](https://retorquere.github.io/zotero-report-customizer/better-bibtex/)

This plugin integrates with (but does not require) [Zotero: Better BibTeX](https://retorquere.github.io/zotero-report-customizer/better-bibtex/), to display the bibtex key plus any conflicts between them.

## Customizing the fields to display

In the generated report, click the pencil to remove fields and change the order and sort. The back arrow reset all current edits, the erase-all (three lines) resets all to default. If the save icon appears that means there are unsaved changes.

## Showing a bibliography rendering instead of the item title

You can replace the title with a bibliography line in the report. The customizer offers a [hidden preference](https://www.zotero.org/support/preferences/hidden_preferences) called `extensions.zotero.report-customizer.bibliography`. If you toggle that to `true`, the title in the report will be replaced with a bibliography rendering according to the default quick-copy format (Prefs - Export - Default Format).

If you want a custom MathJax config, you can add it as a JSON-encoded [configuration block](https://docs.mathjax.org/en/latest/options/input/tex.html?highlight=inlinemath#the-configuration-block) (anything you want, sans the leading `MathJax =` and trailing `;`, in a string preference named `extensions.zotero.report-customizer.MathJax`.

If you want select-links to go to the Zotero website, create a boolean preference named `extensions.zotero.report-customizer.link.web` and set it to `true`.

## Includes indexing status of attachments

(not ported yet to 5.0)

Shows indexing status of attachments, plus links to select attachment

If you experience any problems, or are unclear on how to use it, I'll be glad to [help](https://retorquere.github.io/zotero-report-customizer/support.html).

## **NOTE**

The report customizations must be saved by clicking the Save icon before the report can be saved to disk. I'm looking into this.
