# $NetBSD: Makefile,v 1.11 2021/05/03 19:01:21 pho Exp $

DISTNAME=	X11-xft-0.3.1
PKGREVISION=	6
CATEGORIES=	x11 graphics

MAINTAINER=	esg@sdf.lonestar.org
COMMENT=	Bindings to the Xft library, and some Xrender parts
LICENSE=	gnu-gpl-v2

.include "../../devel/hs-utf8-string/buildlink3.mk"
.include "../../x11/hs-X11/buildlink3.mk"
.include "../../x11/libXft/buildlink3.mk"
.include "../../mk/haskell.mk"
.include "../../mk/bsd.pkg.mk"
