##############################################################################
#
#    file                 : Makefile
#    created              : Wed Jan 8 18:31:16 CET 2003
#    copyright            : (C) 2002-2004 Bernhard Wymann
#    copyright            :          2004 Christos Dimitrakakis
#    email                : berniw@bluewin.ch
#    email                : dimitrak@bluewin.ch
#    version              : $Id: Makefile,v 1.7.2.1 2008/09/03 21:53:38 berniw Exp $
#
##############################################################################
#
#   This program is free software; you can redistribute it and/or modify
#   it under the terms of the GNU General Public License as published by
#   the Free Software Foundation; either version 2 of the License, or
#   (at your option) any later version.
#
##############################################################################

ROBOT       = olethros
MODULE      = ${ROBOT}.so
MODULEDIR   = drivers/${ROBOT}
SOURCES     = ${ROBOT}.cpp driver.cpp opponent.cpp spline.cpp pit.cpp learn.cpp strategy.cpp cardata.cpp geometry.cpp Trajectory.cpp TrackData.cpp
LIBS        = -L${EXPORTBASE}/lib -llearning

SHIPDIR     = drivers/${ROBOT}
SHIP        = ${ROBOT}.xml logo.rgb
SHIPSUBDIRS = 0 2 3 4 5 6 7 9

PKGSUBDIRS  = ${SHIPSUBDIRS}
src-robots-base_PKGFILES = $(shell find * -maxdepth 0 -type f -print)
src-robots-base_PKGDIR   = ${PACKAGE}-${VERSION}/$(subst ${TORCS_BASE},,$(shell pwd))

include ${MAKE_DEFAULT}

#CFLAGSD := $(CFLAGSD) -DUSE_OLETHROS_NAMESPACE
