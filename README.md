# analysis-cpantesters-beforemaintrelease

Trying to reconstruct the page formerly known as http://analysis.cpantesters.org/beforemaintrelease

# Things to know

Each json file potentially contains four figures per versioned distro:

- passes for old perl
- fails for old perl
- passes for new perl
- fails for new perl

The beforemaintrelease page had the following two filters applied:

- ignore distros that had no pass on old perl and no pass on new perl
- ignore distros that had all four figures > 0

This filtering tells potential cpan testers which distros seem worth to
focus on for further analysis. Of very special interest would be those
with only

- passes for old perl
- fails for new perl

Testers should try to focus on those to either produce more data or to
produce evidence that some of them are showstoppers.

# See also

See also: https://github.com/andk/analysis-cpantesters-annotate.git

# COPYRIGHT, LICENCE

Copyright (C) 2018 Andreas König. Licence not yet decided.
