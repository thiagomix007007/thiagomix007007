- 👋 Hi, I’m @thiagomix007007
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
thiagomix007007/thiagomix007007 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

[meu codigo thiago infinitus]


<xml xmlns="http://www.w3.org/1999/xhtml" collection="false">
  <variables>
    <variable type="" id=":WPU,akMBs7bn$VYXx-f">PERDA MÁXIMA</variable>
    <variable type="" id=".9@YH*1NpucHe+jAsdF1">META DE LUCRO</variable>
    <variable type="" id="L4f5`_Bb29Z7N%A:0@yS">VALOR FIXO INICIAL</variable>
    <variable type="" id="5j.nsn;axz$hEm]1G?zv">CONTADOR EVEN</variable>
    <variable type="" id="FfI#0p(tVqi|ffEU+x?~">CONTADOR ODD</variable>
    <variable type="" id="PSK[vpTY1?d,|G1l*lRu">CONTADOR PADRÃO</variable>
    <variable type="" id="X[(S;ATE$Dbs3flXN{-m">STAKE INICIAL</variable>
    <variable type="" id="{_gQ*oKSNI260$_%IiFy">MG COUNT</variable>
    <variable type="" id="ZC9jlKp0p+PVYAU:n7?-">STAKE AO VENCER</variable>
    <variable type="" id=":1(%s`GiXvkUXScRcL9v">RESET</variable>
    <variable type="" id=";wJj_I^Js9-1UR#/~_$1">NEXT TRADE CONDITION</variable>
    <variable type="" id="-Y3Bf$ldt/dlxI4wVJE*">MG 15</variable>
    <variable type="" id="BB7F`v4}r;pEUN_FpAG}">MG 14</variable>
    <variable type="" id="4wHAvdd4n*2MLBb;;C*m">MG 13</variable>
    <variable type="" id="|W^V6Qp;DOgVg?}0{Ze_">MG 1</variable>
    <variable type="" id="Ay:b_!8yf/qT8e*27LCk">MG 12</variable>
    <variable type="" id="0f)_=Gn_l%uh;Y!UQ~G/">MG 2</variable>
    <variable type="" id="IV*Fk*4LHfiAgJ6L2^PE">MG 11</variable>
    <variable type="" id="auG6CaO0fw)vP|w,)]k2">MG 3</variable>
    <variable type="" id="hsx~nm0Ug),(uZJ{6CE3">MG 10</variable>
    <variable type="" id="`G%R{A_mQ=1?k9RcOs/,">MG 4</variable>
    <variable type="" id="]EuekGy%Wf6*BONsh3P6">MG 9</variable>
    <variable type="" id="s(XLY=QF*gwg8ij`mL~:">MG 5</variable>
    <variable type="" id="dZf7=ljtJR+x?{@zY0s{">MG 8</variable>
    <variable type="" id="7W_,cR)pNFtE9-q5/33m">MG 6</variable>
    <variable type="" id="I?elpp]14+7PY2FadTO|">MG 7</variable>
    <variable type="" id="Y]Tv|Tn=/6PU0D|$gcb?">MG 0</variable>
    <variable type="" id="+$d?~d-8=H-`JTUwqM2b">HELP COUNT</variable>
    <variable type="" id="uTz]j:#neq3|^:8gv;n`">COUNT</variable>
  </variables>
  <block type="trade" id="trade" inline="false" collapsed="true" x="0" y="0">
    <field name="MARKET_LIST">synthetic_index</field>
    <field name="SUBMARKET_LIST">random_index</field>
    <field name="SYMBOL_LIST">R_100</field>
    <field name="TRADETYPECAT_LIST">digits</field>
    <field name="TRADETYPE_LIST">evenodd</field>
    <field name="TYPE_LIST">both</field>
    <field name="CANDLEINTERVAL_LIST">60</field>
    <field name="TIME_MACHINE_ENABLED">FALSE</field>
    <field name="RESTARTONERROR">TRUE</field>
    <statement name="INITIALIZATION">
      <block type="variables_set" id="UHbM..aM}w@BeGUT:u[F">
        <field name="VAR" id=":WPU,akMBs7bn$VYXx-f" variabletype="">PERDA MÁXIMA</field>
        <value name="VALUE">
          <block type="text_prompt_ext" id="q[/`(5wvs)ebk(pXOQTJ">
            <mutation type="NUMBER"></mutation>
            <field name="TYPE">NUMBER</field>
            <value name="TEXT">
              <shadow type="text" id="Bmm?xOVBgo)izJG:b/=e">
                <field name="TEXT">Qual o valor de perda máxima iremos tolerar? Recomendação é de 100 (Isso significa que se o robô perder 100 dólares ele automaticamente encerrará as operações!</field>
              </shadow>
            </value>
          </block>
        </value>
        <next>
          <block type="variables_set" id="P4VwO%9`ub#}!|?:Jzgg">
            <field name="VAR" id=".9@YH*1NpucHe+jAsdF1" variabletype="">META DE LUCRO</field>
            <value name="VALUE">
              <block type="text_prompt_ext" id="lVMCD+;/1ND.867r2MG)">
                <mutation type="NUMBER"></mutation>
                <field name="TYPE">NUMBER</field>
                <value name="TEXT">
                  <shadow type="text" id="kUuyQg{v~g,8DaWj;s:Q">
                    <field name="TEXT">Defina a meta de ganhos que iremos buscar? Recomendo que seja de no máximo 5% do valor da sua banca (Ex: Se sua banca for de 100 você deve por 5, pois isso é 5% da sua banca). Faça o calculo de quanto é 5% da sua banca e digite abaixo o valor.</field>
                  </shadow>
                </value>
              </block>
            </value>
            <next>
              <block type="variables_set" id="jE=TS?ooJFBN4f.wswuf" collapsed="true">
                <field name="VAR" id="X[(S;ATE$Dbs3flXN{-m" variabletype="">STAKE INICIAL</field>
                <value name="VALUE">
                  <block type="math_number" id="1llhm%F3?N*?$ch%_wwO">
                    <field name="NUM">0.35</field>
                  </block>
                </value>
                <next>
                  <block type="variables_set" id="dyZV*+tc*@[acK!jCEH`" collapsed="true">
                    <field name="VAR" id="ZC9jlKp0p+PVYAU:n7?-" variabletype="">STAKE AO VENCER</field>
                    <value name="VALUE">
                      <block type="math_number" id="NRTi#47*ai}{!#QMJ=+v">
                        <field name="NUM">0.35</field>
                      </block>
                    </value>
                    <next>
                      <block type="variables_set" id="?O0oSye:vL9eqCi4QqsH" collapsed="true">
                        <field name="VAR" id="L4f5`_Bb29Z7N%A:0@yS" variabletype="">VALOR FIXO INICIAL</field>
                        <value name="VALUE">
                          <block type="math_number" id="Y*wFs:OvyWGl]o?V0[4n">
                            <field name="NUM">0.35</field>
                          </block>
                        </value>
                        <next>
                          <block type="variables_set" id="u%Z;vu)tW$J$0iZ`$%@P" collapsed="true">
                            <field name="VAR" id="-Y3Bf$ldt/dlxI4wVJE*" variabletype="">MG 15</field>
                            <value name="VALUE">
                              <block type="math_number" id="K^bB;)a0$^%l#l7|v=]j">
                                <field name="NUM">15</field>
                              </block>
                            </value>
                            <next>
                              <block type="variables_set" id="o2`52;]BAkuIF3{D;#z_" collapsed="true">
                                <field name="VAR" id="BB7F`v4}r;pEUN_FpAG}" variabletype="">MG 14</field>
                                <value name="VALUE">
                                  <block type="math_number" id="r{@Jh,0c1^+-g=7Sop.g">
                                    <field name="NUM">14</field>
                                  </block>
                                </value>
                                <next>
                                  <block type="variables_set" id="lxj7mJp:@5}sd6Oj)6a4" collapsed="true">
                                    <field name="VAR" id="4wHAvdd4n*2MLBb;;C*m" variabletype="">MG 13</field>
                                    <value name="VALUE">
                                      <block type="math_number" id="OecIoX(CJ_Ie#@P/iOlL">
                                        <field name="NUM">13</field>
                                      </block>
                                    </value>
                                    <next>
                                      <block type="variables_set" id="kSQ8E!Oz:p`!Bu*@qH7}" collapsed="true">
                                        <field name="VAR" id="Ay:b_!8yf/qT8e*27LCk" variabletype="">MG 12</field>
                                        <value name="VALUE">
                                          <block type="math_number" id="`}pKv7KM~MUrxGS}[6:d">
                                            <field name="NUM">12</field>
                                          </block>
                                        </value>
                                        <next>
                                          <block type="variables_set" id="*5Mp8LZ(Tn;oXE2J5Es," collapsed="true">
                                            <field name="VAR" id="IV*Fk*4LHfiAgJ6L2^PE" variabletype="">MG 11</field>
                                            <value name="VALUE">
                                              <block type="math_number" id=".I(XBQM_oPQ7ec8QS`3A">
                                                <field name="NUM">11</field>
                                              </block>
                                            </value>
                                            <next>
                                              <block type="variables_set" id="LS%idN{LdDXn2r=YAT(l" collapsed="true">
                                                <field name="VAR" id="hsx~nm0Ug),(uZJ{6CE3" variabletype="">MG 10</field>
                                                <value name="VALUE">
                                                  <block type="math_number" id="=e=by)yOtMS1iZT7YTA!">
                                                    <field name="NUM">10</field>
                                                  </block>
                                                </value>
                                                <next>
                                                  <block type="variables_set" id="2qfP;#Udnref3O4F^#6G" collapsed="true">
                                                    <field name="VAR" id="]EuekGy%Wf6*BONsh3P6" variabletype="">MG 9</field>
                                                    <value name="VALUE">
                                                      <block type="math_number" id="V=CF2n?8G)_eXzj:4%cI">
                                                        <field name="NUM">9</field>
                                                      </block>
                                                    </value>
                                                    <next>
                                                      <block type="variables_set" id="{g;4nP2exRKr/~M]F,Ek" collapsed="true">
                                                        <field name="VAR" id="dZf7=ljtJR+x?{@zY0s{" variabletype="">MG 8</field>
                                                        <value name="VALUE">
                                                          <block type="math_number" id="$z+d}ZUopDqMmT?@n*_^">
                                                            <field name="NUM">8</field>
                                                          </block>
                                                        </value>
                                                        <next>
                                                          <block type="variables_set" id="~AI]XG`/YXga}%N*ldNt" collapsed="true">
                                                            <field name="VAR" id="I?elpp]14+7PY2FadTO|" variabletype="">MG 7</field>
                                                            <value name="VALUE">
                                                              <block type="math_number" id="TN[[_oFR8Oe?UGY?UCv+">
                                                                <field name="NUM">7</field>
                                                              </block>
                                                            </value>
                                                            <next>
                                                              <block type="variables_set" id=";[pfW^+UeXGOW}Wf1hbJ" collapsed="true">
                                                                <field name="VAR" id="7W_,cR)pNFtE9-q5/33m" variabletype="">MG 6</field>
                                                                <value name="VALUE">
                                                                  <block type="math_number" id="~a_;y}:}c[mDcoDe*H^:">
                                                                    <field name="NUM">6</field>
                                                                  </block>
                                                                </value>
                                                                <next>
                                                                  <block type="variables_set" id="/ZgvW:?4Y$$gU+wav}]," collapsed="true">
                                                                    <field name="VAR" id="s(XLY=QF*gwg8ij`mL~:" variabletype="">MG 5</field>
                                                                    <value name="VALUE">
                                                                      <block type="math_number" id="?Tbuy=m1.=s9?=6)_671">
                                                                        <field name="NUM">5</field>
                                                                      </block>
                                                                    </value>
                                                                    <next>
                                                                      <block type="variables_set" id="_5*e~Tf*}UZ3w`S`%ee{" collapsed="true">
                                                                        <field name="VAR" id="`G%R{A_mQ=1?k9RcOs/," variabletype="">MG 4</field>
                                                                        <value name="VALUE">
                                                                          <block type="math_number" id="W*v)h4!pfl$+a^D4$N9|">
                                                                            <field name="NUM">4</field>
                                                                          </block>
                                                                        </value>
                                                                        <next>
                                                                          <block type="variables_set" id="kfH$GU.I4B/zy3dUGq-R" collapsed="true">
                                                                            <field name="VAR" id="auG6CaO0fw)vP|w,)]k2" variabletype="">MG 3</field>
                                                                            <value name="VALUE">
                                                                              <block type="math_number" id="^:_mSC65B7o|ev~`o.Uz">
                                                                                <field name="NUM">3</field>
                                                                              </block>
                                                                            </value>
                                                                            <next>
                                                                              <block type="variables_set" id="5G4u8wd:rQQJHSL]FOg!" collapsed="true">
                                                                                <field name="VAR" id="0f)_=Gn_l%uh;Y!UQ~G/" variabletype="">MG 2</field>
                                                                                <value name="VALUE">
                                                                                  <block type="math_number" id="6@5X2a,*uWA6-cqL1np,">
                                                                                    <field name="NUM">2</field>
                                                                                  </block>
                                                                                </value>
                                                                                <next>
                                                                                  <block type="variables_set" id="u`b9FkWfz4.-JL6s5et," collapsed="true">
                                                                                    <field name="VAR" id="|W^V6Qp;DOgVg?}0{Ze_" variabletype="">MG 1</field>
                                                                                    <value name="VALUE">
                                                                                      <block type="math_number" id="#hgTmZz:k3N4N]nz@B%S">
                                                                                        <field name="NUM">1</field>
                                                                                      </block>
                                                                                    </value>
                                                                                    <next>
                                                                                      <block type="variables_set" id="$1OlA5[kUM4YK2b.F9Iz" collapsed="true">
                                                                                        <field name="VAR" id="Y]Tv|Tn=/6PU0D|$gcb?" variabletype="">MG 0</field>
                                                                                        <value name="VALUE">
                                                                                          <block type="math_number" id=":f(cQL0u[8M7{_nsi6F|">
                                                                                            <field name="NUM">0</field>
                                                                                          </block>
                                                                                        </value>
                                                                                        <next>
                                                                                          <block type="variables_set" id="!yMoENk6wOssuv+:/.;h" collapsed="true">
                                                                                            <field name="VAR" id="PSK[vpTY1?d,|G1l*lRu" variabletype="">CONTADOR PADRÃO</field>
                                                                                            <value name="VALUE">
                                                                                              <block type="math_number" id="k5t9OXKyG%B1/-HErl8u">
                                                                                                <field name="NUM">0</field>
                                                                                              </block>
                                                                                            </value>
                                                                                            <next>
                                                                                              <block type="variables_set" id="MS8c0zk8.~c)415OazyN" collapsed="true">
                                                                                                <field name="VAR" id="{_gQ*oKSNI260$_%IiFy" variabletype="">MG COUNT</field>
                                                                                                <value name="VALUE">
                                                                                                  <block type="math_number" id="?n=PLQx}g`R@|v@6I$+l">
                                                                                                    <field name="NUM">0</field>
                                                                                                  </block>
                                                                                                </value>
                                                                                                <next>
                                                                                                  <block type="variables_set" id=").(j/rpEiwUV4YGH2j=!" collapsed="true">
                                                                                                    <field name="VAR" id="+$d?~d-8=H-`JTUwqM2b" variabletype="">HELP COUNT</field>
                                                                                                    <value name="VALUE">
                                                                                                      <block type="math_number" id="8#z9$yep8u,}UXQ[1!Gu">
                                                                                                        <field name="NUM">0</field>
                                                                                                      </block>
                                                                                                    </value>
                                                                                                    <next>
                                                                                                      <block type="variables_set" id="|V!vU][[pcgT`dTqj*[0" collapsed="true">
                                                                                                        <field name="VAR" id="uTz]j:#neq3|^:8gv;n`" variabletype="">COUNT</field>
                                                                                                        <value name="VALUE">
                                                                                                          <block type="math_number" id="4jlYiw[jSH0}!y~u9qg:">
                                                                                                            <field name="NUM">1</field>
                                                                                                          </block>
                                                                                                        </value>
                                                                                                        <next>
                                                                                                          <block type="variables_set" id="qoC2@EHrLRA{ed([)GRZ" collapsed="true">
                                                                                                            <field name="VAR" id=":1(%s`GiXvkUXScRcL9v" variabletype="">RESET</field>
                                                                                                            <value name="VALUE">
                                                                                                              <block type="math_number" id="j[/R51(]boSlDFi~ORo~">
                                                                                                                <field name="NUM">0</field>
                                                                                                              </block>
                                                                                                            </value>
                                                                                                            <next>
                                                                                                              <block type="variables_set" id="E)N{E(NmY48Rx{S*%-$2" collapsed="true">
                                                                                                                <field name="VAR" id=";wJj_I^Js9-1UR#/~_$1" variabletype="">NEXT TRADE CONDITION</field>
                                                                                                                <value name="VALUE">
                                                                                                                  <block type="text" id="AsuRHO~]$hd)a#hY:#K]">
                                                                                                                    <field name="TEXT">Even</field>
                                                                                                                  </block>
                                                                                                                </value>
                                                                                                                <next>
                                                                                                                  <block type="notify" id="V$cWM11$*0wJQ95?G$+h" collapsed="true">
                                                                                                                    <field name="NOTIFICATION_TYPE">info</field>
                                                                                                                    <field name="NOTIFICATION_SOUND">silent</field>
                                                                                                                    <value name="MESSAGE">
                                                                                                                      <shadow type="text" id="=3S8WPZb{ftslnW1h~h/">
                                                                                                                        <field name="TEXT">INFINITUS (VIP TRADER)</field>
                                                                                                                      </shadow>
                                                                                                                    </value>
                                                                                                                  </block>
                                                                                                                </next>
                                                                                                              </block>
                                                                                                            </next>
                                                                                                          </block>
                                                                                                        </next>
                                                                                                      </block>
                                                                                                    </next>
                                                                                                  </block>
                                                                                                </next>
                                                                                              </block>
                                                                                            </next>
                                                                                          </block>
                                                                                        </next>
                                                                                      </block>
                                                                                    </next>
                                                                                  </block>
                                                                                </next>
                                                                              </block>
                                                                            </next>
                                                                          </block>
                                                                        </next>
                                                                      </block>
                                                                    </next>
                                                                  </block>
                                                                </next>
                                                              </block>
                                                            </next>
                                                          </block>
                                                        </next>
                                                      </block>
                                                    </next>
                                                  </block>
                                                </next>
                                              </block>
                                            </next>
                                          </block>
                                        </next>
                                      </block>
                                    </next>
                                  </block>
                                </next>
                              </block>
                            </next>
                          </block>
                        </next>
                      </block>
                    </next>
                  </block>
                </next>
              </block>
            </next>
          </block>
        </next>
      </block>
    </statement>
    <statement name="SUBMARKET">
      <block type="tradeOptions" id=")YzxnU6]oSlGh+U)rE;C">
        <field name="DURATIONTYPE_LIST">t</field>
        <field name="CURRENCY_LIST">USD</field>
        <value name="DURATION">
          <block type="math_random_int" id="$H9sxqx`DYFWmvlC.K]=">
            <value name="FROM">
              <shadow type="math_number" id="+so3Wbe3yN);)HS4RW1_">
                <field name="NUM">1</field>
              </shadow>
            </value>
            <value name="TO">
              <shadow type="math_number" id="Qg[Ldt*~NMTp2Zed3xKL">
                <field name="NUM">1</field>
              </shadow>
            </value>
          </block>
        </value>
        <value name="AMOUNT">
          <block type="variables_get" id="7nzOAJqEn6)+OAYI30hM">
            <field name="VAR" id="L4f5`_Bb29Z7N%A:0@yS" variabletype="">VALOR FIXO INICIAL</field>
          </block>
        </value>
      </block>
    </statement>
  </block>
  <block type="before_purchase" id="strategy" collapsed="true" x="0" y="53">
    <statement name="BEFOREPURCHASE_STACK">
      <block type="controls_if" id="83pWD$sFJz8::#[V).j$">
        <mutation elseif="1" else="1"></mutation>
        <value name="IF0">
          <block type="logic_compare" id="OuG91B@P)w:C9QojEC?I">
            <field name="OP">LT</field>
            <value name="A">
              <block type="variables_get" id="hlp-g+/^w5?$|SMMig0~">
                <field name="VAR" id="PSK[vpTY1?d,|G1l*lRu" variabletype="">CONTADOR PADRÃO</field>
              </block>
            </value>
            <value name="B">
              <block type="math_number" id="q|]qvKzQa~nTp/@a)MEd">
                <field name="NUM">2</field>
              </block>
            </value>
          </block>
        </value>
        <statement name="DO0">
          <block type="math_change" id="F-UYB4WJW9mJ392QJNt?">
            <field name="VAR" id="5j.nsn;axz$hEm]1G?zv" variabletype="">CONTADOR EVEN</field>
            <value name="DELTA">
              <shadow type="math_number" id="S#a=o4_n9Fa7`H^YYj2M">
                <field name="NUM">1</field>
              </shadow>
            </value>
            <next>
              <block type="purchase" id="8B~MP)Rc!r@6qrCVNYus">
                <field name="PURCHASE_LIST">DIGITEVEN</field>
              </block>
            </next>
          </block>
        </statement>
        <value name="IF1">
          <block type="logic_operation" id="+V,9isWi2om/6^II/;GG">
            <field name="OP">AND</field>
            <value name="A">
              <block type="logic_compare" id="~S7#[gOjl7LPiC~_B)gw">
                <field name="OP">GTE</field>
                <value name="A">
                  <block type="variables_get" id="?snKqQxZ0f`~Z!ZR}W0q">
                    <field name="VAR" id="PSK[vpTY1?d,|G1l*lRu" variabletype="">CONTADOR PADRÃO</field>
                  </block>
                </value>
                <value name="B">
                  <block type="math_number" id="N5Ls0f[Aq)I^Jf~!RA;f">
                    <field name="NUM">1</field>
                  </block>
                </value>
              </block>
            </value>
            <value name="B">
              <block type="logic_compare" id="ilmTnVK*(Ny8V:LRAj4G">
                <field name="OP">LT</field>
                <value name="A">
                  <block type="variables_get" id="pQ@4gOBo.@f:io`A;2NG">
                    <field name="VAR" id="PSK[vpTY1?d,|G1l*lRu" variabletype="">CONTADOR PADRÃO</field>
                  </block>
                </value>
                <value name="B">
                  <block type="math_number" id="5!dyNseE0!~w0EGRO3Bb">
                    <field name="NUM">4</field>
                  </block>
                </value>
              </block>
            </value>
          </block>
        </value>
        <statement name="DO1">
          <block type="math_change" id=")K5)6Ad8Hm!CQV%dmofh">
            <field name="VAR" id="FfI#0p(tVqi|ffEU+x?~" variabletype="">CONTADOR ODD</field>
            <value name="DELTA">
              <shadow type="math_number" id="x#51qn^6c:2{j;ldwd|a">
                <field name="NUM">1</field>
              </shadow>
            </value>
            <next>
              <block type="purchase" id="QkeI%}i!YN.Tpr/)lCrj">
                <field name="PURCHASE_LIST">DIGITODD</field>
              </block>
            </next>
          </block>
        </statement>
        <statement name="ELSE">
          <block type="variables_set" id="nvt(++),-)26KByIQd8/">
            <field name="VAR" id="PSK[vpTY1?d,|G1l*lRu" variabletype="">CONTADOR PADRÃO</field>
            <value name="VALUE">
              <block type="math_number" id="_:=x(H!H(cks67W-r^Ce">
                <field name="NUM">0</field>
              </block>
            </value>
          </block>
        </statement>
      </block>
    </statement>
  </block>
  <block type="after_purchase" id="finish" collapsed="true" x="0" y="106">
    <statement name="AFTERPURCHASE_STACK">
      <block type="controls_if" id="`B9]s{TClp1*uKm8h0[O">
        <mutation else="1"></mutation>
        <value name="IF0">
          <block type="contract_check_result" id="rEzKK;#|elm3%hwm89id">
            <field name="CHECK_RESULT">loss</field>
          </block>
        </value>
        <statement name="DO0">
          <block type="notify" id="lToYjVh@C.!r{*;wLjt!">
            <field name="NOTIFICATION_TYPE">error</field>
            <field name="NOTIFICATION_SOUND">silent</field>
            <value name="MESSAGE">
              <block type="text_join" id="TLH#c#JuF$,edigN~a,;">
                <mutation items="2"></mutation>
                <value name="ADD0">
                  <block type="text" id="D8+W!1Lf#si]Pg:kKA?A">
                    <field name="TEXT">Perdeu 😩</field>
                  </block>
                </value>
                <value name="ADD1">
                  <block type="read_details" id="Y~A}hQ(k6YyyvwNV9#$z">
                    <field name="DETAIL_INDEX">4</field>
                  </block>
                </value>
              </block>
            </value>
            <next>
              <block type="controls_if" id="TSaQ`n8g-p2ve$NwG|_F">
                <mutation else="1"></mutation>
                <value name="IF0">
                  <block type="logic_compare" id="p7k}sR`xd0juJ~*_pl%W">
                    <field name="OP">EQ</field>
                    <value name="A">
                      <block type="variables_get" id="3MwW^qTo]l](L#{kh|;{">
                        <field name="VAR" id="PSK[vpTY1?d,|G1l*lRu" variabletype="">CONTADOR PADRÃO</field>
                      </block>
                    </value>
                    <value name="B">
                      <block type="logic_null" id="mLdiPM!LBuGI2F)P+h7h"></block>
                    </value>
                  </block>
                </value>
                <statement name="DO0">
                  <block type="math_change" id="n-n34$mzfEbRX]_{qZIq">
                    <field name="VAR" id="X[(S;ATE$Dbs3flXN{-m" variabletype="">STAKE INICIAL</field>
                    <value name="DELTA">
                      <shadow id="N=Vo^MVz~/^(xt7Ag@8E" type="math_number">
                        <field name="NUM">1</field>
                      </shadow>
                      <block type="math_arithmetic" id="HE~,HYL!-JHo`XV`lG32">
                        <field name="OP">MULTIPLY</field>
                        <value name="A">
                          <shadow id="ka8n8|Dugz,q5FkUjs`7" type="math_number">
                            <field name="NUM">1</field>
                          </shadow>
                          <block type="math_single" id="ZU1B2:k15C9L%[hsB3fm">
                            <field name="OP">ABS</field>
                            <value name="NUM">
                              <shadow id="GleSn`9j7Cm7/dqg}FIA" type="math_number">
                                <field name="NUM">9</field>
                              </shadow>
                              <block type="read_details" id="W:[mX.K?_rzri1+4}?d*">
                                <field name="DETAIL_INDEX">4</field>
                              </block>
                            </value>
                          </block>
                        </value>
                        <value name="B">
                          <shadow id="{JXdZCp2%s=sfO@yN:n}" type="math_number">
                            <field name="NUM">1</field>
                          </shadow>
                          <block type="math_number" id="0+7RnE,+uA1P7Ua7v:HO">
                            <field name="NUM">1.071</field>
                          </block>
                        </value>
                      </block>
                    </value>
                    <next>
                      <block type="math_change" id="r4{-et=Sk);/K1;kFET.">
                        <field name="VAR" id="PSK[vpTY1?d,|G1l*lRu" variabletype="">CONTADOR PADRÃO</field>
                        <value name="DELTA">
                          <shadow type="math_number" id="!?+MCJ7NTHD2jIb|jvYG">
                            <field name="NUM">1</field>
                          </shadow>
                        </value>
                      </block>
                    </next>
                  </block>
                </statement>
                <statement name="ELSE">
                  <block type="variables_set" id="vjDU7K;!ll:nn9z@sSR@">
                    <field name="VAR" id="X[(S;ATE$Dbs3flXN{-m" variabletype="">STAKE INICIAL</field>
                    <value name="VALUE">
                      <block type="variables_get" id="Y9Lh3=f;3_)UtN9[;Nb`">
                        <field name="VAR" id="ZC9jlKp0p+PVYAU:n7?-" variabletype="">STAKE AO VENCER</field>
                      </block>
                    </value>
                    <next>
                      <block type="math_change" id="C;cjxi=pQSEe3L_,)USy">
                        <field name="VAR" id="PSK[vpTY1?d,|G1l*lRu" variabletype="">CONTADOR PADRÃO</field>
                        <value name="DELTA">
                          <shadow type="math_number" id="aJZBCp:hg*IPtmg@!eTl">
                            <field name="NUM">1</field>
                          </shadow>
                        </value>
                      </block>
                    </next>
                  </block>
                </statement>
                <next>
                  <block type="controls_if" id="R]qEkuMo[PeRj.|/}FhD">
                    <mutation else="1"></mutation>
                    <value name="IF0">
                      <block type="logic_compare" id="[Y$j_`[3k3iaAS0a2-Mh">
                        <field name="OP">NEQ</field>
                        <value name="A">
                          <block type="variables_get" id="aqlL/r3rkdny]:VI^hPg">
                            <field name="VAR" id=";wJj_I^Js9-1UR#/~_$1" variabletype="">NEXT TRADE CONDITION</field>
                          </block>
                        </value>
                        <value name="B">
                          <block type="text" id="Zq1jB/#=z@mtgR|b;]TI">
                            <field name="TEXT">Even</field>
                          </block>
                        </value>
                      </block>
                    </value>
                    <statement name="DO0">
                      <block type="variables_set" id="H0u=4QuvA7Ck{m-xKqVT">
                        <field name="VAR" id=";wJj_I^Js9-1UR#/~_$1" variabletype="">NEXT TRADE CONDITION</field>
                        <value name="VALUE">
                          <block type="text" id="gK_{rtEPy;H)P%{Z_zo`">
                            <field name="TEXT">Even</field>
                          </block>
                        </value>
                      </block>
                    </statement>
                    <statement name="ELSE">
                      <block type="variables_set" id="BuQahbA7M$E`JEax*TfK">
                        <field name="VAR" id=";wJj_I^Js9-1UR#/~_$1" variabletype="">NEXT TRADE CONDITION</field>
                        <value name="VALUE">
                          <block type="text" id="YSDst9W,5u/}T7Y+!km`">
                            <field name="TEXT">Odd</field>
                          </block>
                        </value>
                      </block>
                    </statement>
                    <next>
                      <block type="math_change" id="KRB)?u(%KgizOP,#YKN9">
                        <field name="VAR" id="{_gQ*oKSNI260$_%IiFy" variabletype="">MG COUNT</field>
                        <value name="DELTA">
                          <shadow type="math_number" id="H?Cf7,ghUe55J[IL~186">
                            <field name="NUM">1</field>
                          </shadow>
                        </value>
                        <next>
                          <block type="controls_if" id="5..LtmEug`tb(NO*F9!M">
                            <value name="IF0">
                              <block type="logic_compare" id="@[jh.#3-NhA5?]1$`rK_">
                                <field name="OP">EQ</field>
                                <value name="A">
                                  <block type="variables_get" id="p8|p?}`uVTXAx]A@fLx9">
                                    <field name="VAR" id="{_gQ*oKSNI260$_%IiFy" variabletype="">MG COUNT</field>
                                  </block>
                                </value>
                                <value name="B">
                                  <block type="variables_get" id="zS$-19hE]~y9TOmQZw!0">
                                    <field name="VAR" id="|W^V6Qp;DOgVg?}0{Ze_" variabletype="">MG 1</field>
                                  </block>
                                </value>
                              </block>
                            </value>
                            <statement name="DO0">
                              <block type="variables_set" id="s3Y7El1_|$5o+f7#t}4|">
                                <field name="VAR" id="L4f5`_Bb29Z7N%A:0@yS" variabletype="">VALOR FIXO INICIAL</field>
                                <value name="VALUE">
                                  <block type="math_number" id="z2yH/OC0Air|I@otk:_w">
                                    <field name="NUM">0.39</field>
                                  </block>
                                </value>
                              </block>
                            </statement>
                            <next>
                              <block type="controls_if" id="2fXID-mKU`kj5bcso4*L">
                                <value name="IF0">
                                  <block type="logic_compare" id="XzrqCa`WdF/_}h1s6zi{">
                                    <field name="OP">EQ</field>
                                    <value name="A">
                                      <block type="variables_get" id="hUa8hvi)gFF{RpaYj@v{">
                                        <field name="VAR" id="{_gQ*oKSNI260$_%IiFy" variabletype="">MG COUNT</field>
                                      </block>
                                    </value>
                                    <value name="B">
                                      <block type="variables_get" id="*-032@}4#J4O-cNPG6ou">
                                        <field name="VAR" id="0f)_=Gn_l%uh;Y!UQ~G/" variabletype="">MG 2</field>
                                      </block>
                                    </value>
                                  </block>
                                </value>
                                <statement name="DO0">
                                  <block type="variables_set" id="5ETC(}kB7}:cD_x1FwTA">
                                    <field name="VAR" id="L4f5`_Bb29Z7N%A:0@yS" variabletype="">VALOR FIXO INICIAL</field>
                                    <value name="VALUE">
                                      <block type="math_number" id="EnW3Hv3^,oX;+=~~0NS@">
                                        <field name="NUM">0.78</field>
                                      </block>
                                    </value>
                                  </block>
                                </statement>
                                <next>
                                  <block type="controls_if" id="!}E_;(*;A8{/Ie8TtpRl">
                                    <value name="IF0">
                                      <block type="logic_compare" id="(#PTql4?A@Yk]Ct3YFkh">
                                        <field name="OP">EQ</field>
                                        <value name="A">
                                          <block type="variables_get" id="$547aVG6#}J2[L_ewVTx">
                                            <field name="VAR" id="{_gQ*oKSNI260$_%IiFy" variabletype="">MG COUNT</field>
                                          </block>
                                        </value>
                                        <value name="B">
                                          <block type="variables_get" id="+a}_:c4ed}ui7C3A*@9L">
                                            <field name="VAR" id="auG6CaO0fw)vP|w,)]k2" variabletype="">MG 3</field>
                                          </block>
                                        </value>
                                      </block>
                                    </value>
                                    <statement name="DO0">
                                      <block type="variables_set" id="^F%Pf`nNTb$%qRp57sx2">
                                        <field name="VAR" id="L4f5`_Bb29Z7N%A:0@yS" variabletype="">VALOR FIXO INICIAL</field>
                                        <value name="VALUE">
                                          <block type="math_number" id="2R9u)zleD^AHQV(((HTY">
                                            <field name="NUM">1.6</field>
                                          </block>
                                        </value>
                                      </block>
                                    </statement>
                                    <next>
                                      <block type="controls_if" id="NCu_vCa{KthSF5k@m6SV">
                                        <value name="IF0">
                                          <block type="logic_compare" id="]d^ea~%+n4P^kEc?936c">
                                            <field name="OP">EQ</field>
                                            <value name="A">
                                              <block type="variables_get" id="ANk6$fdUuQUiF;2n}8[{">
                                                <field name="VAR" id="{_gQ*oKSNI260$_%IiFy" variabletype="">MG COUNT</field>
                                              </block>
                                            </value>
                                            <value name="B">
                                              <block type="variables_get" id="*ZKdQq{w3,?ek2M~#l0G">
                                                <field name="VAR" id="`G%R{A_mQ=1?k9RcOs/," variabletype="">MG 4</field>
                                              </block>
                                            </value>
                                          </block>
                                        </value>
                                        <statement name="DO0">
                                          <block type="variables_set" id="w2b`(f6n.Ez_IUAth9MR">
                                            <field name="VAR" id="L4f5`_Bb29Z7N%A:0@yS" variabletype="">VALOR FIXO INICIAL</field>
                                            <value name="VALUE">
                                              <block type="math_number" id="xlM?tWrx?tHKEj=NhvoG">
                                                <field name="NUM">3.3</field>
                                              </block>
                                            </value>
                                            <next>
                                              <block type="timeout" id="5Oy4M{TZ;|kj*|==xf%U">
                                                <statement name="TIMEOUTSTACK">
                                                  <block type="trade_again" id="ElmMnAj_q]CDE+XNaIdO"></block>
                                                </statement>
                                                <value name="SECONDS">
                                                  <shadow type="math_number" id="vx-RJyK]zN1tu(edA94Z">
                                                    <field name="NUM">1</field>
                                                  </shadow>
                                                  <block type="math_number" id="fN-swiEa}#UTBX_}1XkR">
                                                    <field name="NUM">30</field>
                                                  </block>
                                                </value>
                                              </block>
                                            </next>
                                          </block>
                                        </statement>
                                        <next>
                                          <block type="controls_if" id="Pj]}#CqOtZoE]$Q0:Ux8">
                                            <value name="IF0">
                                              <block type="logic_compare" id="/A)$(gDZ-(yL2V,2F~P8">
                                                <field name="OP">EQ</field>
                                                <value name="A">
                                                  <block type="variables_get" id="2V@th1Z@vN@4*Qs+xaHM">
                                                    <field name="VAR" id="{_gQ*oKSNI260$_%IiFy" variabletype="">MG COUNT</field>
                                                  </block>
                                                </value>
                                                <value name="B">
                                                  <block type="variables_get" id="^vKDfk5~HTdl@=s8W`+$">
                                                    <field name="VAR" id="s(XLY=QF*gwg8ij`mL~:" variabletype="">MG 5</field>
                                                  </block>
                                                </value>
                                              </block>
                                            </value>
                                            <statement name="DO0">
                                              <block type="variables_set" id="5jClob0@d@rUaGq=3_yr">
                                                <field name="VAR" id="L4f5`_Bb29Z7N%A:0@yS" variabletype="">VALOR FIXO INICIAL</field>
                                                <value name="VALUE">
                                                  <block type="math_number" id="]oM9yVsE(fY%6wdrRGhZ">
                                                    <field name="NUM">6.8</field>
                                                  </block>
                                                </value>
                                              </block>
                                            </statement>
                                            <next>
                                              <block type="controls_if" id="BaNm?2n2^6B91IlK,~(O">
                                                <value name="IF0">
                                                  <block type="logic_compare" id="wE|]ib:`C?|A985UzjFm">
                                                    <field name="OP">EQ</field>
                                                    <value name="A">
                                                      <block type="variables_get" id="QBI:K.*FrF9p@711-4_p">
                                                        <field name="VAR" id="{_gQ*oKSNI260$_%IiFy" variabletype="">MG COUNT</field>
                                                      </block>
                                                    </value>
                                                    <value name="B">
                                                      <block type="variables_get" id="`YMzxatCnxErUbb{1]?2">
                                                        <field name="VAR" id="7W_,cR)pNFtE9-q5/33m" variabletype="">MG 6</field>
                                                      </block>
                                                    </value>
                                                  </block>
                                                </value>
                                                <statement name="DO0">
                                                  <block type="variables_set" id="AjhnuVQHEd`HZS=o84$y">
                                                    <field name="VAR" id="L4f5`_Bb29Z7N%A:0@yS" variabletype="">VALOR FIXO INICIAL</field>
                                                    <value name="VALUE">
                                                      <block type="math_number" id="8nCqZ(^7SyVPG_e;9MsM">
                                                        <field name="NUM">13.8</field>
                                                      </block>
                                                    </value>
                                                    <next>
                                                      <block type="timeout" id="R=u~-b*lr-]uu)(XRi6r">
                                                        <statement name="TIMEOUTSTACK">
                                                          <block type="trade_again" id="DD@o^bmXHJ5z4UW#|`Wz"></block>
                                                        </statement>
                                                        <value name="SECONDS">
                                                          <shadow type="math_number" id="vx-RJyK]zN1tu(edA94Z">
                                                            <field name="NUM">1</field>
                                                          </shadow>
                                                          <block type="math_number" id="TW1;PA:V+kRrs@gQ.YXx">
                                                            <field name="NUM">20</field>
                                                          </block>
                                                        </value>
                                                      </block>
                                                    </next>
                                                  </block>
                                                </statement>
                                                <next>
                                                  <block type="controls_if" id="m:;;l6YL.e{YRVC;.0d;">
                                                    <value name="IF0">
                                                      <block type="logic_compare" id="R[B?lAqZ)Tjq(r`4J:xA">
                                                        <field name="OP">EQ</field>
                                                        <value name="A">
                                                          <block type="variables_get" id="bF[1vE4h%rJwyqy_3#SZ">
                                                            <field name="VAR" id="{_gQ*oKSNI260$_%IiFy" variabletype="">MG COUNT</field>
                                                          </block>
                                                        </value>
                                                        <value name="B">
                                                          <block type="variables_get" id="PzC,uZ4!ylybqFRX87)5">
                                                            <field name="VAR" id="I?elpp]14+7PY2FadTO|" variabletype="">MG 7</field>
                                                          </block>
                                                        </value>
                                                      </block>
                                                    </value>
                                                    <statement name="DO0">
                                                      <block type="variables_set" id="h@qVso}~Tx1=mU2OT9gA">
                                                        <field name="VAR" id="L4f5`_Bb29Z7N%A:0@yS" variabletype="">VALOR FIXO INICIAL</field>
                                                        <value name="VALUE">
                                                          <block type="math_number" id="hPCphShYSq_E@P.%RG!Q">
                                                            <field name="NUM">28.6</field>
                                                          </block>
                                                        </value>
                                                      </block>
                                                    </statement>
                                                    <next>
                                                      <block type="controls_if" id="3Srm=gVZ5n{89I_B3e~o">
                                                        <value name="IF0">
                                                          <block type="logic_compare" id="PQDJLTre/fJ.^!/|]iUF">
                                                            <field name="OP">EQ</field>
                                                            <value name="A">
                                                              <block type="variables_get" id="4Y4W=1:m6x$fD3(:y@xH">
                                                                <field name="VAR" id="{_gQ*oKSNI260$_%IiFy" variabletype="">MG COUNT</field>
                                                              </block>
                                                            </value>
                                                            <value name="B">
                                                              <block type="variables_get" id="UI(`Vg}}Wj%K+Ve*idK+">
                                                                <field name="VAR" id="dZf7=ljtJR+x?{@zY0s{" variabletype="">MG 8</field>
                                                              </block>
                                                            </value>
                                                          </block>
                                                        </value>
                                                        <statement name="DO0">
                                                          <block type="variables_set" id="=f6p`B?^zT$]gS8FvcCz">
                                                            <field name="VAR" id="L4f5`_Bb29Z7N%A:0@yS" variabletype="">VALOR FIXO INICIAL</field>
                                                            <value name="VALUE">
                                                              <block type="math_number" id="n?hZn22bj;IUPvktD9El">
                                                                <field name="NUM">58</field>
                                                              </block>
                                                            </value>
                                                            <next>
                                                              <block type="timeout" id="^)-2SU:F9ed]whcbV^gF">
                                                                <statement name="TIMEOUTSTACK">
                                                                  <block type="trade_again" id="]2Y-S|P;yJI@.,3M=t7)"></block>
                                                                </statement>
                                                                <value name="SECONDS">
                                                                  <shadow type="math_number" id="vx-RJyK]zN1tu(edA94Z">
                                                                    <field name="NUM">1</field>
                                                                  </shadow>
                                                                  <block type="math_number" id="LOSiUQ-!Xg_AiQs|HKeF">
                                                                    <field name="NUM">15</field>
                                                                  </block>
                                                                </value>
                                                              </block>
                                                            </next>
                                                          </block>
                                                        </statement>
                                                        <next>
                                                          <block type="controls_if" id="Ix/8HD8ou612Y0Wb!cmZ">
                                                            <value name="IF0">
                                                              <block type="logic_compare" id="g)*s]!WwQJ[P$8A*Qtui">
                                                                <field name="OP">EQ</field>
                                                                <value name="A">
                                                                  <block type="variables_get" id="s=RsNegIL}I;acHhfWi4">
                                                                    <field name="VAR" id="{_gQ*oKSNI260$_%IiFy" variabletype="">MG COUNT</field>
                                                                  </block>
                                                                </value>
                                                                <value name="B">
                                                                  <block type="variables_get" id="}Mqs(4}`s@b:0pikL)3@">
                                                                    <field name="VAR" id="]EuekGy%Wf6*BONsh3P6" variabletype="">MG 9</field>
                                                                  </block>
                                                                </value>
                                                              </block>
                                                            </value>
                                                            <statement name="DO0">
                                                              <block type="variables_set" id="!NG.R:L_[E^(nIc[7U@h">
                                                                <field name="VAR" id="L4f5`_Bb29Z7N%A:0@yS" variabletype="">VALOR FIXO INICIAL</field>
                                                                <value name="VALUE">
                                                                  <block type="math_number" id=":,d?_m4eyim#DUyv-pt#">
                                                                    <field name="NUM">119</field>
                                                                  </block>
                                                                </value>
                                                              </block>
                                                            </statement>
                                                            <next>
                                                              <block type="controls_if" id="Vp!}Y[LE=O=RQhWk}bHm">
                                                                <value name="IF0">
                                                                  <block type="logic_compare" id="7xmt#l-]53+fUDb2rvAy">
                                                                    <field name="OP">EQ</field>
                                                                    <value name="A">
                                                                      <block type="variables_get" id="G?/Np0Z5C99Y1nugx{e(">
                                                                        <field name="VAR" id="{_gQ*oKSNI260$_%IiFy" variabletype="">MG COUNT</field>
                                                                      </block>
                                                                    </value>
                                                                    <value name="B">
                                                                      <block type="variables_get" id="TGDT!gU(!Dq:s^j?;)c4">
                                                                        <field name="VAR" id="hsx~nm0Ug),(uZJ{6CE3" variabletype="">MG 10</field>
                                                                      </block>
                                                                    </value>
                                                                  </block>
                                                                </value>
                                                                <statement name="DO0">
                                                                  <block type="variables_set" id="ig22A,5jjf_xm:EIc{!1">
                                                                    <field name="VAR" id="L4f5`_Bb29Z7N%A:0@yS" variabletype="">VALOR FIXO INICIAL</field>
                                                                    <value name="VALUE">
                                                                      <block type="math_number" id="{h8!]Sg:LpJUV]/Kvehs">
                                                                        <field name="NUM">245</field>
                                                                      </block>
                                                                    </value>
                                                                    <next>
                                                                      <block type="timeout" id="h%Itj`C,8=d_W}v?8209">
                                                                        <statement name="TIMEOUTSTACK">
                                                                          <block type="trade_again" id="~=9=vs({7:)vEy+KX66x"></block>
                                                                        </statement>
                                                                        <value name="SECONDS">
                                                                          <shadow type="math_number" id="vx-RJyK]zN1tu(edA94Z">
                                                                            <field name="NUM">1</field>
                                                                          </shadow>
                                                                          <block type="math_number" id="L3.Pj:J#4~xx]Lnu6wrl">
                                                                            <field name="NUM">10</field>
                                                                          </block>
                                                                        </value>
                                                                      </block>
                                                                    </next>
                                                                  </block>
                                                                </statement>
                                                                <next>
                                                                  <block type="controls_if" id="HGSoO4x:3wyE@LTBt9J}">
                                                                    <value name="IF0">
                                                                      <block type="logic_compare" id="Z8+~zjSv(hLV,UW1Djuv">
                                                                        <field name="OP">EQ</field>
                                                                        <value name="A">
                                                                          <block type="variables_get" id="GhcZBVrv$!gsh3#,Uz2Q">
                                                                            <field name="VAR" id="{_gQ*oKSNI260$_%IiFy" variabletype="">MG COUNT</field>
                                                                          </block>
                                                                        </value>
                                                                        <value name="B">
                                                                          <block type="variables_get" id="T{;T/3/l;A(^VSlog8JR">
                                                                            <field name="VAR" id="IV*Fk*4LHfiAgJ6L2^PE" variabletype="">MG 11</field>
                                                                          </block>
                                                                        </value>
                                                                      </block>
                                                                    </value>
                                                                    <statement name="DO0">
                                                                      <block type="variables_set" id="e$gT!fqk!(~^K2J!Yxq3">
                                                                        <field name="VAR" id="L4f5`_Bb29Z7N%A:0@yS" variabletype="">VALOR FIXO INICIAL</field>
                                                                        <value name="VALUE">
                                                                          <block type="math_number" id="!WVJDWgmd?)lo3dtE1Q?">
                                                                            <field name="NUM">498</field>
                                                                          </block>
                                                                        </value>
                                                                      </block>
                                                                    </statement>
                                                                    <next>
                                                                      <block type="controls_if" id="XhwxnPWk;P2EA],+%Mb?">
                                                                        <value name="IF0">
                                                                          <block type="logic_compare" id="eQ^~#0xp2e~|aR}/E_~B">
                                                                            <field name="OP">EQ</field>
                                                                            <value name="A">
                                                                              <block type="variables_get" id="=YkcP_#`Qp$jJee+k4r3">
                                                                                <field name="VAR" id="{_gQ*oKSNI260$_%IiFy" variabletype="">MG COUNT</field>
                                                                              </block>
                                                                            </value>
                                                                            <value name="B">
                                                                              <block type="variables_get" id="^+`J$^,!Ie-k^F(U}ilL">
                                                                                <field name="VAR" id="Ay:b_!8yf/qT8e*27LCk" variabletype="">MG 12</field>
                                                                              </block>
                                                                            </value>
                                                                          </block>
                                                                        </value>
                                                                        <statement name="DO0">
                                                                          <block type="variables_set" id="J/X~tUdlvXMTjPkL++#^">
                                                                            <field name="VAR" id="L4f5`_Bb29Z7N%A:0@yS" variabletype="">VALOR FIXO INICIAL</field>
                                                                            <value name="VALUE">
                                                                              <block type="math_number" id="cf4qSs,buay~x+NOj??E">
                                                                                <field name="NUM">1020</field>
                                                                              </block>
                                                                            </value>
                                                                            <next>
                                                                              <block type="timeout" id="q)AUh`iz2mg+I4dUp6Lh">
                                                                                <statement name="TIMEOUTSTACK">
                                                                                  <block type="trade_again" id="qJUt9TeLAEeLvM,y/XrV"></block>
                                                                                </statement>
                                                                                <value name="SECONDS">
                                                                                  <shadow type="math_number" id="vx-RJyK]zN1tu(edA94Z">
                                                                                    <field name="NUM">1</field>
                                                                                  </shadow>
                                                                                  <block type="math_number" id="oH;9doAG+A*(^*FU!X=b">
                                                                                    <field name="NUM">5</field>
                                                                                  </block>
                                                                                </value>
                                                                              </block>
                                                                            </next>
                                                                          </block>
                                                                        </statement>
                                                                        <next>
                                                                          <block type="controls_if" id="c5|1L$:S`{$nW16ry*4r">
                                                                            <value name="IF0">
                                                                              <block type="logic_compare" id="}CnH12^y!EWIu-UwBc5O">
                                                                                <field name="OP">EQ</field>
                                                                                <value name="A">
                                                                                  <block type="variables_get" id="=y(zX#kL)~@|pT4t4bVs">
                                                                                    <field name="VAR" id="{_gQ*oKSNI260$_%IiFy" variabletype="">MG COUNT</field>
                                                                                  </block>
                                                                                </value>
                                                                                <value name="B">
                                                                                  <block type="variables_get" id="w}lj}_%QwB|VO]wPQ6Ce">
                                                                                    <field name="VAR" id="4wHAvdd4n*2MLBb;;C*m" variabletype="">MG 13</field>
                                                                                  </block>
                                                                                </value>
                                                                              </block>
                                                                            </value>
                                                                            <statement name="DO0">
                                                                              <block type="variables_set" id="$G+L4^CYc-5}AQq)Bs~w">
                                                                                <field name="VAR" id="L4f5`_Bb29Z7N%A:0@yS" variabletype="">VALOR FIXO INICIAL</field>
                                                                                <value name="VALUE">
                                                                                  <block type="math_number" id="x8FRWIlkMvAbRI}rI9$n">
                                                                                    <field name="NUM">2060</field>
                                                                                  </block>
                                                                                </value>
                                                                              </block>
                                                                            </statement>
                                                                            <next>
                                                                              <block type="controls_if" id="g+b[YfnZnhBNn`d9)(xh">
                                                                                <value name="IF0">
                                                                                  <block type="logic_compare" id="?*DGWE$d*=p.78of8xf?">
                                                                                    <field name="OP">EQ</field>
                                                                                    <value name="A">
                                                                                      <block type="variables_get" id="-/YcP%b|43iEt;Fm-zPy">
                                                                                        <field name="VAR" id="{_gQ*oKSNI260$_%IiFy" variabletype="">MG COUNT</field>
                                                                                      </block>
                                                                                    </value>
                                                                                    <value name="B">
                                                                                      <block type="variables_get" id="JTS2:!{OF?;FvvnhI%i:">
                                                                                        <field name="VAR" id="BB7F`v4}r;pEUN_FpAG}" variabletype="">MG 14</field>
                                                                                      </block>
                                                                                    </value>
                                                                                  </block>
                                                                                </value>
                                                                                <statement name="DO0">
                                                                                  <block type="variables_set" id="Y6pNyP$B7fdK!J~Si/j1">
                                                                                    <field name="VAR" id="L4f5`_Bb29Z7N%A:0@yS" variabletype="">VALOR FIXO INICIAL</field>
                                                                                    <value name="VALUE">
                                                                                      <block type="math_number" id=".w6b/#^Ir_ROj%Ii59-P">
                                                                                        <field name="NUM">4230</field>
                                                                                      </block>
                                                                                    </value>
                                                                                  </block>
                                                                                </statement>
                                                                                <next>
                                                                                  <block type="controls_if" id="XG.5wWEk@Hyf6/Vm%sH|">
                                                                                    <value name="IF0">
                                                                                      <block type="logic_compare" id="!vcEs]t~=r@D*,rW*MYJ">
                                                                                        <field name="OP">EQ</field>
                                                                                        <value name="A">
                                                                                          <block type="variables_get" id="1s%`h3Fm5{CTdd1qK(n2">
                                                                                            <field name="VAR" id="{_gQ*oKSNI260$_%IiFy" variabletype="">MG COUNT</field>
                                                                                          </block>
                                                                                        </value>
                                                                                        <value name="B">
                                                                                          <block type="variables_get" id="_CK#ff6,S|C?/`_-tDbn">
                                                                                            <field name="VAR" id="-Y3Bf$ldt/dlxI4wVJE*" variabletype="">MG 15</field>
                                                                                          </block>
                                                                                        </value>
                                                                                      </block>
                                                                                    </value>
                                                                                    <statement name="DO0">
                                                                                      <block type="variables_set" id=".VD`E17VvT2NB`-C?UkR">
                                                                                        <field name="VAR" id="L4f5`_Bb29Z7N%A:0@yS" variabletype="">VALOR FIXO INICIAL</field>
                                                                                        <value name="VALUE">
                                                                                          <block type="math_number" id="[R|X{Bp$8#8R[e/U7bH0">
                                                                                            <field name="NUM">1</field>
                                                                                          </block>
                                                                                        </value>
                                                                                      </block>
                                                                                    </statement>
                                                                                  </block>
                                                                                </next>
                                                                              </block>
                                                                            </next>
                                                                          </block>
                                                                        </next>
                                                                      </block>
                                                                    </next>
                                                                  </block>
                                                                </next>
                                                              </block>
                                                            </next>
                                                          </block>
                                                        </next>
                                                      </block>
                                                    </next>
                                                  </block>
                                                </next>
                                              </block>
                                            </next>
                                          </block>
                                        </next>
                                      </block>
                                    </next>
                                  </block>
                                </next>
                              </block>
                            </next>
                          </block>
                        </next>
                      </block>
                    </next>
                  </block>
                </next>
              </block>
            </next>
          </block>
        </statement>
        <statement name="ELSE">
          <block type="controls_if" id="[lq{TtU@XYv|X1QJuaom">
            <value name="IF0">
              <block type="contract_check_result" id="[2oF[{4MS@b3Ti8UBn^c">
                <field name="CHECK_RESULT">win</field>
              </block>
            </value>
            <statement name="DO0">
              <block type="variables_set" id="L)1meBt,;bWX+HcyY|jo">
                <field name="VAR" id="{_gQ*oKSNI260$_%IiFy" variabletype="">MG COUNT</field>
                <value name="VALUE">
                  <block type="variables_get" id="FT2ZG_SKodoGhhJ8d+8l">
                    <field name="VAR" id=":1(%s`GiXvkUXScRcL9v" variabletype="">RESET</field>
                  </block>
                </value>
                <next>
                  <block type="variables_set" id="--~k-+^F^{YdkBGf~MqY">
                    <field name="VAR" id="L4f5`_Bb29Z7N%A:0@yS" variabletype="">VALOR FIXO INICIAL</field>
                    <value name="VALUE">
                      <block type="math_number" id=";V?|I#SJ]~%1~}hc9z(j">
                        <field name="NUM">0.35</field>
                      </block>
                    </value>
                    <next>
                      <block type="notify" id="5,dfH~sim}!~aAZXfO]6">
                        <field name="NOTIFICATION_TYPE">success</field>
                        <field name="NOTIFICATION_SOUND">silent</field>
                        <value name="MESSAGE">
                          <block type="text_join" id="QGl0jw%~US:vzq%ep2#g">
                            <mutation items="2"></mutation>
                            <value name="ADD0">
                              <block type="text" id="tA4C=~KucEGJBkJ@o!UP">
                                <field name="TEXT">Acertou 😄</field>
                              </block>
                            </value>
                            <value name="ADD1">
                              <block type="math_single" id="dC}Zi1Mb2e$oZ+G#jhX(">
                                <field name="OP">ABS</field>
                                <value name="NUM">
                                  <shadow id="GleSn`9j7Cm7/dqg}FIA" type="math_number">
                                    <field name="NUM">9</field>
                                  </shadow>
                                  <block type="read_details" id="pC+hir|cp!y*VT:$t!{g">
                                    <field name="DETAIL_INDEX">4</field>
                                  </block>
                                </value>
                              </block>
                            </value>
                          </block>
                        </value>
                        <next>
                          <block type="variables_set" id="5Z{NQT9x,sQ*:s[0g=^Q">
                            <field name="VAR" id="X[(S;ATE$Dbs3flXN{-m" variabletype="">STAKE INICIAL</field>
                            <value name="VALUE">
                              <block type="variables_get" id="/)JFAMbLm%Nk4(!JK)8B">
                                <field name="VAR" id="ZC9jlKp0p+PVYAU:n7?-" variabletype="">STAKE AO VENCER</field>
                              </block>
                            </value>
                            <next>
                              <block type="controls_if" id="TA4uy0qs*w!T=Fnu!W24" collapsed="true">
                                <mutation else="1"></mutation>
                                <value name="IF0">
                                  <block type="logic_compare" id="1dt5pzBV$8$7fEBD2.6T">
                                    <field name="OP">NEQ</field>
                                    <value name="A">
                                      <block type="variables_get" id="k@W)Rl;Q/?S9XX+n6|*v">
                                        <field name="VAR" id=";wJj_I^Js9-1UR#/~_$1" variabletype="">NEXT TRADE CONDITION</field>
                                      </block>
                                    </value>
                                    <value name="B">
                                      <block type="text" id="=4{sY5?n[0JwinOxt`%9">
                                        <field name="TEXT">Even</field>
                                      </block>
                                    </value>
                                  </block>
                                </value>
                                <statement name="DO0">
                                  <block type="variables_set" id="EOWNuW9`~$U!DRoT0[+Q">
                                    <field name="VAR" id=";wJj_I^Js9-1UR#/~_$1" variabletype="">NEXT TRADE CONDITION</field>
                                    <value name="VALUE">
                                      <block type="text" id="U1Xp3xpK6DCHsS6kYN!q">
                                        <field name="TEXT">Even</field>
                                      </block>
                                    </value>
                                  </block>
                                </statement>
                                <statement name="ELSE">
                                  <block type="variables_set" id="FPillj1)CZ.E^`?$O*tD">
                                    <field name="VAR" id=";wJj_I^Js9-1UR#/~_$1" variabletype="">NEXT TRADE CONDITION</field>
                                    <value name="VALUE">
                                      <block type="text" id="P`Iq,aIdjiH|fwYEMyn7">
                                        <field name="TEXT">Odd</field>
                                      </block>
                                    </value>
                                  </block>
                                </statement>
                              </block>
                            </next>
                          </block>
                        </next>
                      </block>
                    </next>
                  </block>
                </next>
              </block>
            </statement>
          </block>
        </statement>
        <next>
          <block type="notify" id="jqtqq%8EV{w?[%[hAl8K">
            <field name="NOTIFICATION_TYPE">info</field>
            <field name="NOTIFICATION_SOUND">silent</field>
            <value name="MESSAGE">
              <block type="text_join" id="C`v-o;eI-F0lx[kI[d@=">
                <mutation items="2"></mutation>
                <value name="ADD0">
                  <block type="text" id="gHX]4-3[;aU;nft#`*y:">
                    <field name="TEXT">Total 💲:</field>
                  </block>
                </value>
                <value name="ADD1">
                  <block type="total_profit" id="1qsU.~gXA$4YcS/FWd=Y"></block>
                </value>
              </block>
            </value>
            <next>
              <block type="controls_if" id=".yAfxZz%M[+3*Fd=R)=M">
                <mutation else="1"></mutation>
                <value name="IF0">
                  <block type="logic_compare" id="]2`@pj.Q`qCA1n5Yw|2Q">
                    <field name="OP">LT</field>
                    <value name="A">
                      <block type="total_profit" id="3#mxU/b~yj)/B}cW1pf|"></block>
                    </value>
                    <value name="B">
                      <block type="variables_get" id="sBQc:L:@L5HOpx6F=l{y">
                        <field name="VAR" id=".9@YH*1NpucHe+jAsdF1" variabletype="">META DE LUCRO</field>
                      </block>
                    </value>
                  </block>
                </value>
                <statement name="DO0">
                  <block type="controls_if" id="^l1azJHKQ$orJ-q]lG0Q">
                    <mutation else="1"></mutation>
                    <value name="IF0">
                      <block type="logic_operation" id="h8v_zq%rg77(5OK2$)^[">
                        <field name="OP">AND</field>
                        <value name="A">
                          <block type="math_number_property" id="#A4?Z6#|{3DN(?XsZh@F">
                            <mutation divisor_input="false"></mutation>
                            <field name="PROPERTY">NEGATIVE</field>
                            <value name="NUMBER_TO_CHECK">
                              <shadow id="otH_VG.6ad,:GnG=3=)5" type="math_number">
                                <field name="NUM">0</field>
                              </shadow>
                              <block type="total_profit" id="kylMakAh08%mw:*nPaau"></block>
                            </value>
                          </block>
                        </value>
                        <value name="B">
                          <block type="logic_compare" id="1*XklJatRfP`}k+HifCm">
                            <field name="OP">GTE</field>
                            <value name="A">
                              <block type="math_single" id=")c#_,HP;A8a~GVrD,Iwe">
                                <field name="OP">ABS</field>
                                <value name="NUM">
                                  <shadow id="(UBCH+RQSwYPbgf%@ANZ" type="math_number">
                                    <field name="NUM">9</field>
                                  </shadow>
                                  <block type="total_profit" id="Tg(#~RUo1/W.`)1Xwu~#"></block>
                                </value>
                              </block>
                            </value>
                            <value name="B">
                              <block type="variables_get" id="/t[^=+u0i2Xm~Ij{NZwv">
                                <field name="VAR" id=":WPU,akMBs7bn$VYXx-f" variabletype="">PERDA MÁXIMA</field>
                              </block>
                            </value>
                          </block>
                        </value>
                      </block>
                    </value>
                    <statement name="DO0">
                      <block type="text_print" id="S84|^~ejd~*byDCJ?*jt">
                        <value name="TEXT">
                          <shadow id="Nau%l+%*hH!#y2I#Q@%5" type="text">
                            <field name="TEXT">abc</field>
                          </shadow>
                          <block type="text" id="*$)}hFOMKc#Q3q(R8c:N">
                            <field name="TEXT">❌ Infelizmente fomos stopados, mas amanhã é outro dia! ❌</field>
                          </block>
                        </value>
                      </block>
                    </statement>
                    <statement name="ELSE">
                      <block type="trade_again" id=";xc0RFP.I}X3~me9hBg+"></block>
                    </statement>
                  </block>
                </statement>
                <statement name="ELSE">
                  <block type="text_print" id="-e/Xlr?f`NIR]F.tWW0l">
                    <value name="TEXT">
                      <shadow id="kqlrIk.GO.^}hI,PoUV)" type="text">
                        <field name="TEXT">abc</field>
                      </shadow>
                      <block type="text_join" id="78zEFur}Qx??GXjak-Z-">
                        <mutation items="2"></mutation>
                        <value name="ADD0">
                          <block type="text" id="$]oX6-Opz56KO_yU*3dY">
                            <field name="TEXT">✅ META BATIDA&lt; AGORA VÁ CUIDAR DA SUA FAMÍLIA ✅</field>
                          </block>
                        </value>
                        <value name="ADD1">
                          <block type="total_profit" id="sBvouo.nD;(6gaU5C7wM"></block>
                        </value>
                      </block>
                    </value>
                  </block>
                </statement>
              </block>
            </next>
          </block>
        </next>
      </block>
    </statement>
  </block>
</xml>
