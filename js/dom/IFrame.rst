IFrame - HTML iframe
==================================================

.. py:class:: IFrame()

    Наследник :py:class:`Element`


    .. py:attribute:: contentDocument
        
        До­ку­мент :py:class:`Document`, со­дер­жа­щий дан­ный эле­мент <iframe>. Ес­ли до­ку­мент ото­бра­жа­ет­ся в <iframe> с дру­гим про­ис­хо­ж­де­ни­ем, дос­туп к этому до­ку­мен­ту бу­дет за­крыт из-за ог­ра­ни­че­ний, на­кла­ды­вае­мых по­ли­ти­кой об­ще­го про­ис­хо­ж­де­ния.


    .. py:attribute:: contentWindow
        
        Объ­ект :py:class:`Window`, со­дер­жа­щий эле­мент <iframe>. (Свой­ст­во frameElement это­го объ­ек­та Window бу­дет ссы­лать­ся об­рат­но на дан­ный объ­ект IFrame.)


    .. py:attribute:: height
        
        Вы­со­та эле­мен­та <iframe> в  CSS-пик­се­лах. Это свой­ст­во со­от­вет­ст­ву­ет ат­ри­бу­ту height.


    .. py:attribute:: name
        
        Имя эле­мен­та <iframe>. Это свой­ст­во со­от­вет­ст­ву­ет ат­ри­бу­ту name, а  его зна­че­ние мож­но при­сваи­вать свой­ст­ву target объ­ек­тов Link и Form.


    .. py:attribute:: sandbox
        
        Это свой­ст­во со­от­вет­ст­ву­ет HTML5-ат­ри­бу­ту sandbox и мо­жет ис­поль­зо­вать­ся как стро­ка или как мно­же­ст­во от­дель­ных лек­сем.
        
        Ат­ри­бут sandbox оп­ре­де­ля­ет, ка­кие до­пол­ни­тель­ные ог­ра­ни­че­ния долж­ны на­кла­ды­вать­ся бро­узе­ром на со­дер­жи­мое, ото­бра­жае­мое в эле­мен­те <iframe>. Ес­ли ат­ри­бут sandbox при­сут­ст­ву­ет в эле­мен­те, но име­ет пус­тое зна­че­ние, со­дер­жи­мое фрей­ма <iframe> бу­дет ин­тер­пре­ти­ро­вать­ся как имею­щее дру­гое про­ис­хо­ж­де­ние, и ему не бу­дет по­зво­ле­но за­пус­кать сце­на­рии, ото­бра­жать фор­мы и  из­ме­нять свой­ст­во location ок­на, со­дер­жа­ще­го фрейм. Ат­ри­бу­ту sandbox мож­но так­же при­сво­ить спи­сок лек­сем, раз­де­лен­ных про­бе­ла­ми, сни­маю­щих эти до­пол­ни­тель­ные ог­ра­ни­че­ния. До­пус­ти­мы­ми лек­се­ма­ми яв­ля­ют­ся: «allow-same-origin», «allow-scripts», «al­low-forms» и «allow-top-navigation».

        
    .. py:attribute:: seamless
        
        Это свой­ст­во со­от­вет­ст­ву­ет ат­ри­бу­ту seamless. Ес­ли оно име­ет зна­че­ние true, бро­узер дол­жен ото­бра­жать со­дер­жи­мое эле­мен­та <iframe> так, как ес­ли бы оно бы­ло со­став­ной ча­стью объ­ем­лю­ще­го до­ку­мен­та. От­час­ти это оз­на­ча­ет, что бро­узер дол­жен при­ме­нить к со­дер­жи­мо­му фрей­ма сти­ли CSS вме­щаю­ще­го до­ку­мен­та.
        
        Ат­ри­бут seamless был вве­ден в спе­ци­фи­ка­ции HTML5 и на мо­мент на­пи­са­ния этих строк был реа­ли­зо­ван не во всех бро­узе­рах.


    .. py:attribute:: src
        
        Это свой­ст­во со­от­вет­ст­ву­ет ат­ри­бу­ту src эле­мен­та <iframe>: он оп­ре­де­ля­ет URL-ад­рес со­дер­жи­мо­го фрей­ма.


    .. py:attribute:: srcdoc
        
        Это свой­ст­во со­от­вет­ст­ву­ет ат­ри­бу­ту srcdoc и  оп­ре­де­ля­ет со­дер­жи­мое эле­мен­та <iframe> в ви­де стро­ки. Ат­ри­бут srcdoc был вве­ден в спе­ци­фи­ка­ции HTML5 со­всем не­дав­но и на мо­мент на­пи­са­ния этих строк был реа­ли­зо­ван не во всех бро­узе­рах.


.. py:attribute:: width

    Ши­ри­на фрей­ма в CSS-пик­се­лах. Это свой­ст­во со­от­вет­ст­ву­ет ат­ри­бу­ту width.