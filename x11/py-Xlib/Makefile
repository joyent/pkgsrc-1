# $NetBSD: Makefile,v 1.16 2020/12/19 16:56:34 prlw1 Exp $

DISTNAME=	python-xlib-0.29
PKGNAME=	${PYPKGPREFIX}-${DISTNAME:S/python-x/X/}
CATEGORIES=	x11
MASTER_SITES=	${MASTER_SITE_GITHUB:=python-xlib/}
GITHUB_PROJECT=	python-xlib
GITHUB_RELEASE=	${PKGVERSION_NOREV}
EXTRACT_SUFX=	.tar.bz2

MAINTAINER=	prlw1@cam.ac.uk
HOMEPAGE=	https://github.com/python-xlib/python-xlib/
COMMENT=	XLib in pure Python
LICENSE=	gnu-lgpl-v2.1

USE_LANGUAGES=	# none

DEPENDS+=	${PYPKGPREFIX}-setuptools_scm-[0-9]*:../../devel/py-setuptools_scm
DEPENDS+=	${PYPKGPREFIX}-six-[0-9]*:../../lang/py-six

.include "../../lang/python/egg.mk"
.include "../../mk/bsd.pkg.mk"
