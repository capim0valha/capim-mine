```jsx
import React, { useState } from 'react';

export default function App() {
  const [activeTab, setActiveTab] = useState('home');
  const [isMenuOpen, setIsMenuOpen] = useState(false);

  return (
    <div className="bg-gray-900 text-white min-h-screen">
      {/* Header */}
      <header className="bg-gray-800 shadow-md sticky top-0 z-50">
        <div className="container mx-auto px-4 py-4 flex justify-between items-center">
          <div className="flex items-center space-x-2">
            <svg className="w-8 h-8 text-green-500" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2">
              <path d="M4 16l4.586-4.586a2 2 2 0 012.828 0L16 16m-2-2l1.586-1.586a2 2 2 0 012.828 0L20 14" strokeLinecap="round" strokeLinejoin="round" />
              <path d="M16 16v2a2 2 2 0 01-2 2H6a2 2 2 0 01-2-2v-7.586l2 2V18h8v-2z" strokeLinecap="round" strokeLinejoin="round" />
              <path d="M20 8v6M16 8v6" strokeLinecap="round" strokeLinejoin="round" />
            </svg>
            <h1 className="text-xl font-bold text-green-400">MineServer</h1>
          </div>

          {/* Desktop Navigation */}
          <nav className="hidden md:flex space-x-8">
            <button 
              onClick={() => setActiveTab('home')} 
              className={`py-2 transition-colors ${activeTab === 'home' ? 'text-green-400 border-b-2 border-green-400' : 'hover:text-green-300'}`}
            >
              Home
            </button>
            <button 
              onClick={() => setActiveTab('about')} 
              className={`py-2 transition-colors ${activeTab === 'about' ? 'text-green-400 border-b-2 border-green-400' : 'hover:text-green-300'}`}
            >
              Sobre
            </button>
            <button 
              onClick={() => setActiveTab('rules')} 
              className={`py-2 transition-colors ${activeTab === 'rules' ? 'text-green-400 border-b-2 border-green-400' : 'hover:text-green-300'}`}
            >
              Regras
            </button>
            <button 
              onClick={() => setActiveTab('contact')} 
              className={`py-2 transition-colors ${activeTab === 'contact' ? 'text-green-400 border-b-2 border-green-400' : 'hover:text-green-300'}`}
            >
              Contato
            </button>
          </nav>

          {/* Mobile Menu Button */}
          <button 
            className="md:hidden text-gray-300 hover:text-white"
            onClick={() => setIsMenuOpen(!isMenuOpen)}
          >
            <svg className="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              {isMenuOpen ? (
                <path strokeLinecap="round" strokeLinejoin="round" strokeWidth="2" d="M6 18L18 6M6 6l12 12" />
              ) : (
                <path strokeLinecap="round" strokeLinejoin="round" strokeWidth="2" d="M4 6h16M4 12h16M4 18h16" />
              )}
            </svg>
          </button>
        </div>

        {/* Mobile Menu */}
        {isMenuOpen && (
          <div className="md:hidden bg-gray-700 px-4 py-2 space-y-2">
            <button 
              onClick={() => { setActiveTab('home'); setIsMenuOpen(false); }} 
              className={`block w-full text-left py-2 transition-colors ${activeTab === 'home' ? 'text-green-400' : 'hover:text-green-300'}`}
            >
              Home
            </button>
            <button 
              onClick={() => { setActiveTab('about'); setIsMenuOpen(false); }} 
              className={`block w-full text-left py-2 transition-colors ${activeTab === 'about' ? 'text-green-400' : 'hover:text-green-300'}`}
            >
              Sobre
            </button>
            <button 
              onClick={() => { setActiveTab('rules'); setIsMenuOpen(false); }} 
              className={`block w-full text-left py-2 transition-colors ${activeTab === 'rules' ? 'text-green-400' : 'hover:text-green-300'}`}
            >
              Regras
            </button>
            <button 
              onClick={() => { setActiveTab('contact'); setIsMenuOpen(false); }} 
              className={`block w-full text-left py-2 transition-colors ${activeTab === 'contact' ? 'text-green-400' : 'hover:text-green-300'}`}
            >
              Contato
            </button>
          </div>
        )}
      </header>

      {/* Main Content */}
      <main className="container mx-auto px-4 py-8">
        {activeTab === 'home' && (
          <section className="text-center">
            <h2 className="text-4xl md:text-5xl font-bold mb-6 text-green-400">Bem-vindo ao MineServer</h2>
            <p className="text-lg md:text-xl mb-8 text-gray-300 max-w-2xl mx-auto">
              Um servidor Minecraft seguro, divertido e sempre atualizado. Jogue com amigos e explore nosso mundo criativo!
            </p>
            
            <div className="mb-12">
              <div className="bg-gray-800 p-6 rounded-lg shadow-lg inline-block">
                <h3 className="text-xl font-semibold mb-4">Status do Servidor</h3>
                <div className="flex items-center justify-center space-x-2">
                  <div className="w-3 h-3 rounded-full bg-green-500 animate-pulse"></div>
                  <span className="text-green-400 font-medium">Online</span>
                </div>
                <p className="mt-2 text-sm text-gray-400">IP: play.mineserver.com.br</p>
              </div>
            </div>

            <div className="grid md:grid-cols-3 gap-8">
              <div className="bg-gray-800 p-6 rounded-lg shadow-lg hover:shadow-green-500/20 transition-shadow">
                <div className="text-green-400 mb-4">
                  <svg className="w-12 h-12 mx-auto" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2">
                    <path d="M19 21V5a2 2 0 00-2-2H7a2 2 0 00-2 2v16m14 0h2m-2 0h-5m-9 0H3m2 0h5M9 7h1m-1 4h1m4-4h1m-1 4h1m-5 10v-5a1 1 0 011-1h2a1 1 0 011 1v5m-4 0h4" strokeLinecap="round" strokeLinejoin="round" />
                  </svg>
                </div>
                <h4 className="text-lg font-semibold mb-2">Modos de Jogo</h4>
                <p className="text-gray-300">Sobrevivência, Criativo, Parkour, SkyBlock e mais!</p>
              </div>

              <div className="bg-gray-800 p-6 rounded-lg shadow-lg hover:shadow-green-500/20 transition-shadow">
                <div className="text-green-400 mb-4">
                  <svg className="w-12 h-12 mx-auto" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2">
                    <path d="M17 20h5v-2a3 3 0 00-5.356-1.857M17 20H7m10 0v-2c0-.656-.126-1.283-.356-1.857M7 20H2v-2a3 3 0 015.356-1.857M7 20v-2c0-.656.126-1.283.356-1.857m0 0a5.002 5.002 0 019.288 0M15 7a3 3 0 11-6 0 3 3 0 016 0zm6 3a2 2 0 11-4 0 2 2 0 014 0zM7 10a2 2 0 11-4 0 2 2 0 014 0z" strokeLinecap="round" strokeLinejoin="round" />
                  </svg>
                </div>
                <h4 className="text-lg font-semibold mb-2">Comunidade Ativa</h4>
                <p className="text-gray-300">Mais de 1000 jogadores online diariamente.</p>
              </div>

              <div className="bg-gray-800 p-6 rounded-lg shadow-lg hover:shadow-green-500/20 transition-shadow">
                <div className="text-green-400 mb-4">
                  <svg className="w-12 h-12 mx-auto" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2">
                    <path d="M12 6V4m0 2a2 2 0 100 4m0-4a2 2 0 110 4m-6 8a2 2 0 100-4m0 4a2 2 0 110-4m0 4v2m0-6V4m6 6v10m6-2a2 2 0 100-4m0 4a2 2 0 110-4m0 4v2m0-6V4" strokeLinecap="round" strokeLinejoin="round" />
                  </svg>
                </div>
                <h4 className="text-lg font-semibold mb-2">Atualizações Frequentes</h4>
                <p className="text-gray-300">Sempre atualizado com as últimas versões do Minecraft.</p>
              </div>
            </div>
          </section>
        )}

        {activeTab === 'about' && (
          <section className="max-w-3xl mx-auto">
            <h2 className="text-3xl font-bold mb-6 text-green-400">Sobre o MineServer</h2>
            
            <div className="bg-gray-800 p-6 rounded-lg shadow-lg mb-8">
              <h3 className="text-xl font-semibold mb-4">Nossa História</h3>
              <p className="text-gray-300 mb-4">
                Fundado em 2020, o MineServer nasceu da paixão por Minecraft e da necessidade de criar um espaço seguro e divertido para todos os jogadores.
              </p>
              <p className="text-gray-300">
                Hoje somos um dos maiores servidores do Brasil, com milhares de jogadores ativos e uma comunidade incrível que cresce cada dia mais.
              </p>
            </div>

            <div className="grid md:grid-cols-2 gap-6 mb-8">
              <div className="bg-gray-800 p-6 rounded-lg shadow-lg">
                <h3 className="text-lg font-semibold mb-3 text-green-400">Nossa Missão</h3>
                <p className="text-gray-300">
                  Criar um ambiente inclusivo e divertido onde todos possam explorar, construir e se divertir com amigos, sem preocupações.
                </p>
              </div>
              <div className="bg-gray-800 p-6 rounded-lg shadow-lg">
                <h3 className="text-lg font-semibold mb-3 text-green-400">Nossa Visão</h3>
                <p className="text-gray-300">
                  Ser o maior e melhor servidor de Minecraft do Brasil, oferecendo sempre novidades e atualizações para melhorar a experiência dos jogadores.
                </p>
              </div>
            </div>

            <div className="bg-gray-800 p-6 rounded-lg shadow-lg">
              <h3 className="text-xl font-semibold mb-4">Nossa Equipe</h3>
              <div className="grid grid-cols-2 md:grid-cols-4 gap-4">
                {['Admin', 'Moderador', 'Desenvolvedor', 'Criador de Conteúdo'].map((role, index) => (
                  <div key={index} className="text-center">
                    <div className="w-16 h-16 mx-auto mb-2 bg-gray-700 rounded-full flex items-center justify-center">
                      <span className="text-gray-300">👤</span>
                    </div>
                    <p className="text-sm text-gray-300">{role}</p>
                  </div>
                ))}
              </div>
            </div>
          </section>
        )}

        {activeTab === 'rules' && (
          <section className="max-w-3xl mx-auto">
            <h2 className="text-3xl font-bold mb-6 text-green-400">Regras do Servidor</h2>
            
            <div className="bg-gray-800 p-6 rounded-lg shadow-lg mb-6">
              <h3 className="text-xl font-semibold mb-4">Regras Gerais</h3>
              <ul className="space-y-3">
                <li className="flex items-start">
                  <span className="text-green-400 mr-2">✔</span>
                  <span className="text-gray-300">Respeite todos os jogadores, evite ofensas e discriminação.</span>
                </li>
                <li className="flex items-start">
                  <span className="text-green-400 mr-2">✔</span>
                  <span className="text-gray-300">Não use mods ou hacks que dêem vantagem injusta.</span>
                </li>
                <li className="flex items-start">
                  <span className="text-green-400 mr-2">✔</span>
                  <span className="text-gray-300">Não construa ou compartilhe conteúdo inapropriado.</span>
                </li>
                <li className="flex items-start">
                  <span className="text-green-400 mr-2">✔</span>
                  <span className="text-gray-300">Não compartilhe sua conta com ninguém.</span>
                </li>
                <li className="flex items-start">
                  <span className="text-green-400 mr-2">✔</span>
                  <span className="text-gray-300">Siga as instruções da equipe de administração.</span>
                </li>
              </ul>
            </div>

            <div className="bg-gray-800 p-6 rounded-lg shadow-lg mb-6">
              <h3 className="text-xl font-semibold mb-4">Regras de Construção</h3>
              <ul className="space-y-3">
                <li className="flex items-start">
                  <span className="text-green-400 mr-2">✔</span>
                  <span className="text-gray-300">Não construa estruturas que obstruam o caminho dos outros.</span>
                </li>
                <li className="flex items-start">
                  <span className="text-green-400 mr-2">✔</span>
                  <span className="text-gray-300">Não construa em áreas que não sejam suas ou públicas.</span>
                </li>
                <li className="flex items-start">
                  <span className="text-green-400 mr-2">✔</span>
                  <span className="text-gray-300">Evite construir com blocos excessivamente chamativos.</span>
                </li>
              </ul>
            </div>

            <div className="bg-gray-800 p-6 rounded-lg shadow-lg">
              <h3 className="text-xl font-semibold mb-4">Regras de Chat</h3>
              <ul className="space-y-3">
                <li className="flex items-start">
                  <span className="text-green-400 mr-2">✔</span>
                  <span className="text-gray-300">Não envie mensagens repetidas ou spam.</span>
                </li>
                <li className="flex items-start">
                  <span className="text-green-400 mr-2">✔</span>
                  <span className="text-gray-300">Não compartilhe links externos sem permissão.</span>
                </li>
                <li className="flex items-start">
                  <span className="text-green-400 mr-2">✔</span>
                  <span className="text-gray-300">Não use linguagem ofensiva ou vulgar.</span>
                </li>
              </ul>
            </div>
          </section>
        )}

        {activeTab === 'contact' && (
          <section className="max-w-3xl mx-auto">
            <h2 className="text-3xl font-bold mb-6 text-green-400">Fale Conosco</h2>
            
            <div className="bg-gray-800 p-6 rounded-lg shadow-lg mb-8">
              <h3 className="text-xl font-semibold mb-4">Entre em Contato</h3>
              <p className="text-gray-300 mb-6">
                Tem dúvidas, sugestões ou precisa de ajuda? Envie uma mensagem para nossa equipe e responderemos o mais rápido possível.
              </p>
              
              <form className="space-y-4">
                <div>
                  <label htmlFor="name" className="block text-sm font-medium text-gray-300 mb-1">Nome</label>
                  <input 
                    type="text" 
                    id="name" 
                    className="w-full px-4 py-2 bg-gray-700 border border-gray-600 rounded-md focus:outline-none focus:ring-2 focus:ring-green-500"
                    placeholder="Seu nome"
                  />
                </div>
                
                <div>
                  <label htmlFor="email" className="block text-sm font-medium text-gray-300 mb-1">Email</label>
                  <input 
                    type="email" 
                    id="email" 
                    className="w-full px-4 py-2 bg-gray-700 border border-gray-600 rounded-md focus:outline-none focus:ring-2 focus:ring-green-500"
                    placeholder="seu@email.com"
                  />
                </div>
                
                <div>
                  <label htmlFor="message" className="block text-sm font-medium text-gray-300 mb-1">Mensagem</label>
                  <textarea 
                    id="message" 
                    rows="5" 
                    className="w-full px-4 py-2 bg-gray-700 border border-gray-600 rounded-md focus:outline-none focus:ring-2 focus:ring-green-500"
                    placeholder="Digite sua mensagem..."
                  ></textarea>
                </div>
                
                <button 
                  type="submit" 
                  className="w-full bg-green-600 hover:bg-green-700 text-white font-medium py-2 px-4 rounded-md transition-colors"
                >
                  Enviar Mensagem
                </button>
              </form>
            </div>

            <div className="grid md:grid-cols-3 gap-6">
              <div className="bg-gray-800 p-6 rounded-lg shadow-lg text-center">
                <div className="text-green-400 mb-3">
                  <svg className="w-8 h-8 mx-auto" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2">
                    <path d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z" strokeLinecap="round" strokeLinejoin="round" />
                  </svg>
                </div>
                <h4 className="text-lg font-semibold mb-1">Telefone</h4>
                <p className="text-gray-300">(11) 99999-9999</p>
              </div>

              <div className="bg-gray-800 p-6 rounded-lg shadow-lg text-center">
                <div className="text-green-400 mb-3">
                  <svg className="w-8 h-8 mx-auto" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2">
                    <path d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" strokeLinecap="round" strokeLinejoin="round" />
                  </svg>
                </div>
                <h4 className="text-lg font-semibold mb-1">Email</h4>
                <p className="text-gray-300">contato@mineserver.com.br</p>
              </div>

              <div className="bg-gray-800 p-6 rounded-lg shadow-lg text-center">
                <div className="text-green-400 mb-3">
                  <svg className="w-8 h-8 mx-auto" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2">
                    <path d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z" strokeLinecap="round" strokeLinejoin="round" />
                    <path d="M15 11a3 3 0 11-6 0 3 3 0 016 0z" strokeLinecap="round" strokeLinejoin="round" />
                  </svg>
                </div>
                <h4 className="text-lg font-semibold mb-1">Localização</h4>
                <p className="text-gray-300">São Paulo, SP - Brasil</p>
              </div>
            </div>
          </section>
        )}
      </main>

      {/* Footer */}
      <footer className="bg-gray-800 py-8">
        <div className="container mx-auto px-4">
          <div className="flex flex-col md:flex-row justify-between items-center">
            <div className="flex items-center space-x-2 mb-4 md:mb-0">
              <svg className="w-6 h-6 text-green-400" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2">
                <path d="M4 16l4.586-4.586a2 2 0 012.828 0L16 16m-2-2l1.586-1.586a2 2 0 012.828 0L20 14" strokeLinecap="round" strokeLinejoin="round" />
                <path d="M16 16v2a2 2 0 01-2 2H6a2 2 0 01-2-2v-7.586l2 2V18h8v-2z" strokeLinecap="round" strokeLinejoin="round" />
                <path d="M20 8v6M16 8v6" strokeLinecap="round" strokeLinejoin="round" />
              </svg>
              <span className="text-lg font-bold text-green-400">MineServer</span>
            </div>
            
            <div className="flex space-x-4">
              <a href="#" className="text-gray-400 hover:text-green-400 transition-colors">
                <span className="sr-only">Instagram</span>
                <svg className="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                  <path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zM12 0C8.741 0 8.333.014 7.053.072 2.695.272.273 2.69.073 7.052.014 8.333 0 8.741 0 12c0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98C8.333 23.986 8.741 24 12 24c3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.668-.072-4.948-.196-4.354-2.617-6.78-6.979-6.98C15.668.014 15.259 0 12 0zm0 5.838a6.162 6.162 0 100 12.324 6.162 6.162 0 000-12.324zM12 16a4 4 0 110-8 4 4 0 010 8zm6.406-11.845a1.44 1.44 0 100 2.881 1.44 1.44 0 000-2.881z" />
                </svg>
              </a>
              <a href="#" className="text-gray-400 hover:text-green-400 transition-colors">
                <span className="sr-only">Discord</span>
                <svg className="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                  <path d="M20.317 4.477a17.839 17.839 0 00-4.71-1.506 17.33 17.33 0 00-3.434.473 1.618 1.618 0 00-1.362.97c-.415.832-.81 2.138-.97 3.022a12.716 12.716 0 00-3.746 0 11.437 11.437 0 00-.96-3.023 1.623 1.623 0 00-1.363-.97A17.327 17.327 0 003.69 4.477a17.77 17.77 0 00-1.51 4.67 18.05 18.05 0 00-1.517 4.67 18.11 18.11 0 001.49 6.333 18.646 18.646 0 004.68 5.754 17.88 17.88 0 003.31.478 17.38 17.38 0 001.593.094c.54-.063 1.065-.195 1.572-.385a1.58 1.58 0 00.92-1.474c.006-.136.01-.273.01-.41a12.46 12.46 0 003.02-1.243 1.61 1.61 0 00.622-1.364c.02-.38-.07-.753-.26-1.087a1.55 1.55 0 00-1.315-.733 12.24 12.24 0 00-3.755-2.23 12.4 12.4 0 00.71-2.11 13.2 13.2 0 0011.15-2.176 18.03 18.03 0 001.48-4.67 17.93 17.93 0 00-.003-4.67zm-9.81 12.21c-.897 0-1.623-.81-1.623-1.807 0-.997.726-1.807 1.623-1.807.896 0 1.623.81 1.623 1.807 0 .997-.727 1.807-1.623 1.807zm5.45 0c-.897 0-1.623-.81-1.623-1.807 0-.997.726-1.807 1.623-1.807.896 0 1.623.81 1.623 1.807 0 .997-.727 1.807-1.623 1.807z" />
                </svg>
              </a>
              <a href="#" className="text-gray-400 hover:text-green-400 transition-colors">
                <span className="sr-only">YouTube</span>
                <svg className="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                  <path d="M23.498 6.186a3.016 3.016 0 00-2.122-2.136C19.505 3.545 12 3.545 12 3.545s-7.505 0-9.377.505A3.017 3.017 0 00.502 6.186C0 8.07 0 12 0 12s0 3.93.502 5.814a3.016 3.016 0 002.122 2.136c1.871.505 9.376.505 9.376.505s7.505 0 9.377-.505a3.015 3.015 0 002.122-2.136C24 15.93 24 12 24 12s0-3.93-.502-5.814zM9.545 15.568V8.432L15.818 12l-6.273 3.568z" />
                </svg>
              </a>
            </div>
          </div>
          
          <div className="mt-8 pt-6 border-t border-gray-700 text-center text-gray-400 text-sm">
            <p>&copy; 2025 MineServer. Todos os direitos reservados.</p>
          </div>
        </div>
      </footer>
    </div>
  );
}
```
