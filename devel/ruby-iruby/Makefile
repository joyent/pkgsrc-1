# $NetBSD: Makefile,v 1.4 2021/05/29 15:04:31 taca Exp $

DISTNAME=	iruby-0.7.0
CATEGORIES=	devel

MAINTAINER=	ryoon@NetBSD.org
HOMEPAGE=	https://github.com/SciRuby/iruby
COMMENT=	Ruby kernel for Jupyter/IPython frontends
LICENSE=	mit

DEPENDS+=	${RUBY_PKGPREFIX}-bond>=0.5.1:../../devel/ruby-bond
DEPENDS+=	${RUBY_PKGPREFIX}-data_uri>=0.1.0:../../www/ruby-data_uri
DEPENDS+=	${RUBY_PKGPREFIX}-mime-types>=3.3.1:../../mail/ruby-mime-types
DEPENDS+=	${RUBY_PKGPREFIX}-multi_json>=1.11:../../textproc/ruby-multi_json

DEPENDS+=	${RUBY_PKGPREFIX}-pycall>=1.3.1:../../devel/ruby-pycall
DEPENDS+=	${RUBY_PKGPREFIX}-fiddle-[0-9]*:../../devel/ruby-fiddle
DEPENDS+=	${RUBY_PKGPREFIX}-ffi-rzmq-[0-9]*:../../net/ruby-ffi-rzmq

DEPENDS+=	${PYPKGPREFIX}-ipython>=6.0.0:../../devel/py-ipython

USE_LANGUAGES=	# none

RUBYGEM_OPTIONS+=	--format-executable

SUBST_CLASSES+=		python
SUBST_STAGE.python=	pre-configure
SUBST_MESSAGE.python=	Versioned ipython command
SUBST_FILES.python=	lib/iruby/command.rb
SUBST_VARS.python=	PYVERSSUFFIX

.include "../../lang/ruby/gem.mk"
.include "../../lang/python/pyversion.mk"
.include "../../mk/bsd.pkg.mk"
