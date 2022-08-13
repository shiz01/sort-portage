#!/bin/bash

for dir in /etc/portage/{package.accept_keywords,package.env,package.license,package.mask,package.unmask,package.use,sets}; do
    pushd "${dir}"; # &> /dev/null;
    for item in *; do
          cat "${item}" | sort -u | sort > "${item}.sorted_file" && mv "${item}.sorted_file" "${item}" -v;
    done
    popd; # &> /dev/null;
done


