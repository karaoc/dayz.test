TODO.

	override bool CanObjectAttach( Object obj )
	{
		if ( !obj.IsInherited( PlayerBase ) ) 
			return false;

		if ( vector.Distance( GetPosition(), obj.GetPosition() ) > m_BoundingRadius * 1.5 )
			return false;

		return true;
	}