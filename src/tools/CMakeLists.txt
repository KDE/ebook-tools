# SPDX-FileCopyrightText: 2007-2008 Ely Levy <elylevy@cs.huji.ac.il>
# SPDX-FileCopyrightText: 2008 Pino Toscano <pino@kde.org>
#
# SPDX-License-Identifier: MIT

include_directories (${EBOOK-TOOLS_SOURCE_DIR}/src/libepub)
add_executable (einfo einfo.c)
target_link_libraries (einfo epub)    

install ( TARGETS einfo DESTINATION bin )
if(NOT WIN32)
  install ( PROGRAMS lit2epub DESTINATION bin )
endif(NOT WIN32)
