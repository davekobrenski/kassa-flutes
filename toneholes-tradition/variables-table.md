What follows is a series of tools and charts I’ve developed over the course of my flute-making journey, to aid in the calculation of tonehole placement for a 3-hole Fulani Flute made from uniform diameter tube. 

While this “electronic worksheet” is the result of honing my process with many dozens of flutes, the concepts and equations are based largely on those outlined in Bart Hopkin’s [Air Columns and Toneholes: Principles for Wind Instrument Design][1] — a fabulous resource for aspiring flutemakers and enthusiasts alike. That resource has proven to be invaluable to me numerous times as I searched for answers as to why a particular flute was slightly off, or while continuously striving to improve upon a prior prototype. I share the below information in the hopes that it may be of some benefit (or at least some interest) to someone else out there embarking on a similar path.

<p class="highlight-text bg-info">
<i class="fa fa-info-circle"></i> If you know what you're doing and want <em>just</em> the tools with no background information, <a href="flute-calc">click here</a>.</p>

[1]:http://windworld.com/products-page/books-cds/air-columns-and-toneholes-principles-for-wind-instrument-design/
[2]:flute-calc

##Background Information

###Variables

In order to properly calculate the placement of toneholes on a flute, several variables come into play. They are:

<table class="table table-striped">
				<tbody>
					<tr>
						<td>\( L_{eff} \)</td>
						<td>The <strong>effective tube length</strong> associated with each desired note. This is the length the flute would be <em>theoretically</em> if it were &ldquo;uncomplicated by end corrections, toneholes, and the like&rdquo; (Hopkin, p.18). For flutes that are open at both ends (the blowhole constitutes an open end), this length is equal to the ½ the actual wavelength of the note itself.</td>
					</tr>
					<tr>
						<td>\( v_{sound} \)</td>
						<td>the <strong>speed of sound</strong> in air, which varies depending on the temperature and the humidity of the air. Since our variable \( L_{eff} \) above is equal to ½ the wavelength of a given note, we need \( v_{sound} \) to be able to calculate the wavelength of that note. (We&rsquo;ll automatically calculate the speed of sound for our environment below.)</td>
					</tr>
					<tr>
						<td>\( A \)</td>
						<td>The <strong>actual tube length</strong> of the desired lowest note of the flute. We use the <em>effective</em> tube length \( L_{eff} \), above, to <em>estimate</em> the actual length — but we won&rsquo;t know the <em>actual</em> length of the flute until we have reduced the flute&rsquo;s length down until it produces the correct note. We need the actual length of <em>just the lowest note</em>, however, in order to accurately position the rest of our toneholes using the <em>tonehole correction factor</em>, that we will calculate below.</td>
					</tr>
					
					<tr>
						<td>\( C \)</td>
						<td>The <strong>tonehole correction factor</strong> — this is really the crux of the matter and what we are after; it is the amount the hole position must be displaced from the effective tube length (above), given the variables that follow:</td>
					</tr>
					
					<tr>
						<td>\( d_t \)</td>
						<td>the <strong>internal diameter</strong> of the tube</td>
					</tr>
					
					<tr>
						<td>\( d_h \)</td>
						<td>the <strong>diameter of the tonehole(s)</strong></td>
					</tr>
					
					<tr>
						<td>\( t_e \)</td>
						<td>the <strong><em>effective</em> thickness of the tonehole</strong> (this is the flute&rsquo;s wall thickness <em>plus</em> some end corrections that depend on the diameter of the hole). \( t_e\ =\ t\ +\ .75d_h \)</td>
					</tr>
					
					<tr>
						<td>\( s \)</td>
						<td>the distance between \( L_{eff} \) for the hole in question and \( L_{eff} \) for the next hole below (or the entire tube in the case of the first open hole)</td>
					</tr>
					
				</tbody>
			</table>
