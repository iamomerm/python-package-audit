## <ins> Package Audit </ins>

Python Package Audit is a lightweight static analysis tool designed to detect unused Python packages in a given project directory <br>
It helps developers clean up their environments by identifying which packages are installed but not used—reducing bloat, <br>
improving dependency hygiene, and speeding up deployments <br>

*Warning - Ignored directories starting with "." or "_" !* <br>
*Warning - Unused package detection is not guaranteed to be accurate !* <br>
*Warning -  It is highly recommended to review the results carefully before removing any packages !* <br>

### <ins> Features </ins>

- Scans Python files to detect all imported modules
- Maps import names to actual installed PyPI packages
- Tracks both direct and transitive dependencies
- Flags packages that are installed but unused
- Provides optional JSON output for automation pipelines
- Ignores common noise (E.G. folders starting with "." or "_")
- Multithreaded for fast analysis of large projects

### <ins> Installation </ins>

You can install this package via PIP: pip install python-package-audit <br>

### <ins> Dependencies </ins>

This project requires the following Python packages:
- colorama — For colored terminal output
- pipdeptree — For analyzing package dependency trees

### <ins> Usage </ins>

python pkgaudit.py --project "/path/to/your/project-root-directory" <br>

### <ins> JSON Output </ins>

python pkgaudit.py --project "/path/to/your/project-root-directory" --json <br>
