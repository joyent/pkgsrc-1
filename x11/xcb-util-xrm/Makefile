# $NetBSD: Makefile,v 1.4 2019/11/03 09:14:19 rillig Exp $

DISTNAME=	xcb-util-xrm-1.3
CATEGORIES=	x11
MASTER_SITES=	${MASTER_SITE_GITHUB:=Airblader/}
GITHUB_RELEASE=	v${PKGVERSION_NOREV}

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	https://github.com/Airblader/xcb-util-xrm/
COMMENT=	XCB utility functions for the X resource manager
LICENSE=	x11

GNU_CONFIGURE=	yes
USE_LIBTOOL=	yes
USE_TOOLS+=	gm4 pkg-config

PKGCONFIG_OVERRIDE=	xcb-xrm.pc.in

.include "../../devel/xorg-util-macros/buildlink3.mk"
.include "../../x11/libX11/buildlink3.mk"
.include "../../x11/xcb-util/buildlink3.mk"

.include "../../mk/bsd.pkg.mk"
